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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405323"
---
# <a name="app-registration-owner-issues"></a>ปัญหาเจ้าของการลงทะเบียนแอป

ต่อไปนี้คือวิธีที่พร้อมใช้งานในการเพิ่มเงินต้นในฐานะเจ้าของในการลงทะเบียนแอป:

- การใช้โมดูล Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    การอ้างอิง: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- การใช้ Azure CLI - `az ad app owner add`

    การอ้างอิง: [เจ้าของแอป Az Ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- การใช้ MS Graph -

    การอ้างอิง: [เพิ่มเจ้าของ - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- การใช้พอร์ทัล Azure AD - นําทางไปยัง [portal.azure.com>](https://portal.azure.com/) Azure Active Directory >การลงทะเบียนแอป>เลือกแอปพลิเคชัน>เจ้าของ>เพิ่มเจ้าของ

**ไม่สามารถดูแอปพลิเคชันของคุณบนใบลงทะเบียนแอปได้ แม้ว่าคุณจะเป็นเจ้าของแอปพลิเคชันนั้นหรือไม่**

เจ้าของแอปไม่ใช่บทบาทการจัดการ ถ้าการตั้งค่า [จํากัดการเข้าถึงพอร์ทัลการดูแลระบบ Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) ถูกเปิดใช้งาน เฉพาะผู้ดูแลระบบเท่านั้นที่สามารถดูแอปพลิเคชันบนพอร์ทัลการลงทะเบียนแอปได้ เพื่อให้เจ้าของสามารถดูแอปพลิเคชันได้ ให้ปิดใช้งานการตั้งค่านี้ (ตั้งค่านี้เป็น NO) หรือกําหนดบทบาทผู้ดูแลระบบให้เจ้าของเฉพาะแอปพลิเคชันที่ระบุเท่านั้น However for this, you will require an Azure AD Premium P2 license and [enable Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
