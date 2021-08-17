---
title: รับรายการของแอปพลิเคชัน Enterprise
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116747"
---
# <a name="get-a-list-of-enterprise-applications"></a>รับรายการของแอปพลิเคชัน Enterprise

1. เมื่อต้องการรับ **รายการ** แอปพลิเคชันขององค์กร (แอปพลิเคชันทั้งหมดหรือถูกกรองตามชื่อที่ใช้แสดง, ID, URI ของตัวระบุ และอื่นๆ) ผ่านทางสั่ง Powershell ให้ดู [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. เมื่อต้องการรับรายการของวัตถุหลักบริการ (วัตถุทั้งหมดหรือถูกกรองตาม ID) ผ่านสั่ง Powershell ให้ดู[Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. ถ้าคุณต้องการดูรายการ **แอปที่กําหนดค่า SAML สคริปต์ PowerShell ต่อไปนี้** อาจช่วยคุณได้:

    แอปพลิเคชันทั้งหมดจะเป็นแอป OAuth หรือแอป SAML (ทั้งแกลเลอรีและแอปที่ไม่อยู่ในแกลเลอรี) จะมีวัตถุสองรายการที่สร้างขึ้นใน AAD เมื่อการลงทะเบียนของพวกเขาเกิดขึ้น วัตถุหนึ่งเรียกว่า วัตถุ Application และอีกวัตถุหนึ่งคือวัตถุ Service Principal เมื่อคุณรวมคุณสมบัติของวัตถุหลักบริการโดยใช้ PowerShell คุณจะพบว่าแอปพลิเคชันทุกรายการมีแท็กที่เกี่ยวข้องกับแอปพลิเคชันนั้นจํานวนหนึ่ง ดังนี้

    - แอป OAuth จะมีแท็กที่เรียกว่า "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    ดังนั้นคุณสามารถใช้แท็กเหล่านี้และค้นหาชนิดของแอปได้ แท็ก "**WindowsAzureActiveDirectoryIntegratedApp**" เป็นปกติของแอปทุกประเภท คุณสามารถใช้ส่วนย่อยต่อไปนี้เพื่อแสดงรายการแอป SAML ทั้งหมด (ทั้งแกลเลอรีและแอปที่ไม่อยู่ในแกลเลอรี):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    หากต้องการข้อมูลเพิ่มเติม โปรดดู[ระบุแอปที่เปิดใช้งาน SAML ใน Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **ค้นหาและแสดงรายการแอปพลิเคชันบนเว็บเท่านั้น**: ใช้สั่งด้านล่างเพื่อรับแอปพลิเคชัน Azure AD ทั้งหมดที่มีประเภทแอปพลิเคชัน "เว็บแอป/API"

    Get-AzureADApplication -ทั้งหมด:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **ค้นหาและแสดงรายการแอปพลิเคชันดั้งเดิมอย่างเดียว**: เรียกใช้สั่งต่อไปนี้เพื่อรับแอปพลิเคชันไคลเอ็นต์ดั้งเดิม (เดสก์ท็อป/อุปกรณ์เคลื่อนที่) ทั้งหมด

    Get-AzureADApplication -ทั้งหมด:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **ส่งออกรายละเอียดแอปพลิเคชัน Azure AD ที่ลงทะเบียนทั้งหมดเป็น CSV:** สั่งด้านล่างจะส่งออกแอป Azure AD ทั้งหมดที่มีรายละเอียดที่ต้องมีเป็นไฟล์ CSV:

    - Get-AzureADApplication -ทั้งหมด:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **ต้องการส่งออกรายการแอป Azure ที่ไม่ได้ใช้** - รายงานการตรวจสอบ

    Azure AD สามารถแสดงบันทึกแอปพลิเคชันได้ภายในเวลาเพียง 30 วันเมื่อคุณมีสิทธิ์การใช้งาน Azure AD Premiumได้
    คุณมีสองตัวเลือกในการเก็บข้อมูลให้นานกว่า 30 วัน คุณสามารถใช้ API [การรายงานของ Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) เพื่อดึงข้อมูลทางโปรแกรมและจัดเก็บในฐานข้อมูล อีกวิธีหนึ่งคือ คุณสามารถรวมบันทึกการตรวจสอบลงในระบบของบริษัทอื่นของ

    คุณยังสามารถดาวน์โหลดรายการแอปของแอปพลิเคชันทั้งหมดและแอปพลิเคชันที่เป็นเจ้าของภายใต้ การลงทะเบียน>Active Directory ของ Azure Active Directory>ดาวน์โหลด>แอปพลิเคชันทั้งหมด/แอปพลิเคชันที่เป็นเจ้าของ

    เมื่อต้องการรับรายการแอปพลิเคชันผ่าน MS Graph ให้ดู[แอปพลิเคชันรายการ - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list)และ[ชนิดของทรัพยากรแอปพลิเคชัน - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application)
