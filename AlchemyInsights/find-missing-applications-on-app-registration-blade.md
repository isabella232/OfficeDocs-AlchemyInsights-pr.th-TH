---
title: ค้นหาแอปพลิเคชันที่หายไปบนใบลงทะเบียนแอป
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
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057121"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>ค้นหาแอปพลิเคชันที่หายไปบนใบลงทะเบียนแอป

1. ไม่พบแอปพลิเคชันบนพอร์ทัลการลงทะเบียนแอป

    ถ้าแอปพลิเคชันเป็นแอปพลิเคชันแบบหลายผู้เช่าและลงทะเบียนในผู้เช่าอื่น แอปพลิเคชันนั้นจะไม่แสดงภายใต้ ใบลงทะเบียนแอป อย่างไรก็ตาม คุณอาจพบภายใต้ใบแอปพลิเคชัน Enterprise เมื่อเข้าถึง (หลังจากได้รับความยินยอม) และหลักบริการถูกสร้างขึ้นในผู้เช่าของคุณแล้ว For more information, see [Apps & service principals in Azure AD - แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. ไม่สามารถดูแอปในใบลงทะเบียนแอปได้ แม้ว่าคุณจะเป็นผู้ดูแลระบบ

    โปรดตรวจสอบให้แน่ใจว่าคุณอยู่ในไดเรกทอรีที่ถูกต้องบนพอร์ทัล Azure
3. แอปพลิเคชันของฉันไม่แสดงอยู่ภายใต้ใบแอปพลิเคชัน Enterprise แต่จะแสดงขึ้นเมื่อฉันคิวรีสั่ง PowerShell

    ในบางครั้ง หลังจากที่คุณลบแอปพลิเคชันจากพอร์ทัล Azure แอปพลิเคชันนั้นจะไม่แสดงขึ้นในพอร์ทัล แต่อาจไม่ถูกลบออกทั้งหมด สำหรับข้อมูลเพิ่มเติม ให้ดู:
    - คุณสามารถเรียกใช้รายการของแอปพลิเคชันที่ถูกลบก่อนหน้า และดูว่าแอปพลิเคชันแสดงขึ้นในรายการโดยใช้สั่ง Powershell: **Get-AzureADDeletedApplication** เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - ถ้าคุณต้องการเอาแอปพลิเคชันออกอย่างสมบูรณ์ คุณสามารถลองต่อไปนี้ใน PowerShell: **Remove-AzureADApplication -ObjectId** เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - อีกวิธีหนึ่งคือ คุณสามารถลองคืนค่าแอปพลิเคชันที่ถูกลบโดยใช้การสั่ง Powershell ต่อไปนี้: คืนค่า **AzureADDeletedApplication -ObjectId** เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[คืนค่า-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. ไม่พบรายการแอปพลิเคชันองค์กรที่ติดตั้งไว้ล่วงหน้าทั้งหมดในผู้เช่า Azure ใหม่ของฉัน

    ไม่มีแอปพลิเคชันขององค์กรที่ติดตั้งไว้ล่วงหน้าใน Azure AD ตามค่าเริ่มต้น คุณต้องเพิ่มด้วยตนเองจากตัวเลือก 'แอปพลิเคชันใหม่' โดยการเรียกดูจากแกลเลอรี Azure AD หรือเพิ่มแอปพลิเคชันที่ไม่ใช่แกลเลอรี เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[การเริ่มต้นใช้งานด่วน: เพิ่มแอปพลิเคชันลงในผู้เช่า Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)ของคุณ
    ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง คุณสามารถเข้าถึงแอปของคุณโดยใช้ตัวเปิดใช้แอปของ[Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)ได้อย่างง่ายดาย
5. ไม่พบแอปของฉันจากพอร์ทัลแอปของฉัน

    ตรวจสอบให้แน่ใจว่าแอปไม่ได้ซ่อนอยู่ในหน้าคอลเลกชัน แอปของฉัน เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู คอลเลกชัน (ตัวอย่าง) ในพอร์ทัลแอปของฉัน - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. เมื่อต้องการเริ่มต้นแอปจากพอร์ทัล แอปของฉัน ให้ดู[&แอปบนพอร์ทัลแอปของฉัน - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 แอปตัวย้ายไม่แสดงบนใบแอปพลิเคชันขององค์กรหลังจากการติดตั้ง

    แอปพลิเคชัน "Office 365 Mover" เป็นแอปแบบหลายผู้เนรการที่ไม่ต้องการเพิ่มลงใน AAD โดยใช้ส่วน แอปพลิเคชันแกลเลอรี ภายใต้ การลงทะเบียนแอปขององค์กร เมื่อต้องการOffice 365แอปผู้ย้าย เพียงแค่ลงชื่อเข้าใช้แอป และขอความยินยอมจากผู้ใช้เกี่ยวกับสิทธิ์ เมื่อผู้ใช้ให้ความยินยอม แอปนี้จะถูกเพิ่มลงในผู้เช่าโดยอัตโนมัติด้วยรหัสอีเมลที่คุณเข้าสู่ระบบ

    หลังจากลงชื่อเข้าใช้แอปพลิเคชัน คุณควรจะสามารถค้นหารายการของแอปพลิเคชันนี้ภายใต้เบลดของแอปพลิเคชัน Enterprise ใน AAD คุณต้องค้นหาแอปพลิเคชันโดยพิมพ์ชื่อเต็ม เช่น "Office 365 Mover" หรือค้นหา "office" และควรแสดงรายการแอป เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดู Office 365 Mover ระบุว่ามีการติดตั้งอยู่แล้ว แต่ไม่ได้แสดงรายการอยู่ในแกลเลอรีแอปพลิเคชันระดับ](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)องค์กร
8. คู่มือเริ่มต้นใช้งานด่วน: ดูรายการแอปพลิเคชันที่ใช้ผู้เช่า[Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)ของคุณเพื่อดูการจัดการข้อมูลเฉพาะตัวแสดงวิธีการดูแอปพลิเคชัน หรือที่เรียกว่าแอปที่ตั้งค่าให้ใช้ผู้เช่า Azure AD เป็นผู้ให้บริการข้อมูลเฉพาะตัว (IdP) อยู่แล้ว
9. [แก้ไขปัญหาทั่วไปในการเพิ่มหรือเอาแอปพลิเคชันออกAzure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps)ช่วยให้คุณเข้าใจปัญหาทั่วไปที่ผู้คนดูแอปAzure Active Directoryแอป
