---
title: ปัญหาเจ้าของการลงทะเบียนแอป
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951152"
---
# <a name="app-registration-owner-issues"></a>ปัญหาเจ้าของการลงทะเบียนแอป

ต่อไปนี้คือวิธีการเพิ่มหลักที่พร้อมใช้งานในฐานะเจ้าของในการลงทะเบียนแอป:

- การใช้โมดูล PowerShell ของ Azure AD -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    การอ้างอิง: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- การใช้ Azure CLI - `az ad app owner add`

    การอ้างอิง: [เจ้าของแอป az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- การใช้ MS Graph -

    การอ้างอิง:[เพิ่มเจ้าของ - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- การใช้พอร์ทัล Azure AD - นําทาง [portal.azure.com>การลงทะเบียน](https://portal.azure.com/) > Azure Active Directory > เลือกแอปพลิเคชัน>เจ้าของ>เพิ่มเจ้าของ

**ไม่สามารถดูแอปพลิเคชันของคุณบนใบลงทะเบียนแอปได้ แม้ว่าคุณจะเป็นเจ้าของแอปพลิเคชันนั้นอยู่ใช่หรือไม่**

เจ้าของแอปไม่ใช่บทบาทผู้ดูแลระบบ ถ้าเปิดใช้งาน [การตั้งค่า จํากัดการเข้าถึงพอร์ทัลการดูแล](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) ระบบ Azure AD เฉพาะผู้ดูแลระบบเท่านั้นที่สามารถดูแอปพลิเคชันบนพอร์ทัลการลงทะเบียนแอปได้ เพื่อให้เจ้าของสามารถดูแอปพลิเคชันได้ ให้ปิดใช้งานการตั้งค่านี้ (ตั้งค่าเป็น ไม่ใช่) หรือกําหนดบทบาทผู้ดูแลระบบให้เจ้าของเฉพาะแอปพลิเคชันที่ระบุเท่านั้น อย่างไรก็ตาม คุณจะต้องมีสิทธิ์การใช้งาน Azure AD Premium P2 และเปิดใช้งาน[Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
