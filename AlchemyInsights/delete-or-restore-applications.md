---
title: ลบหรือคืนค่าแอปพลิเคชัน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102590"
---
# <a name="delete-or-restore-applications"></a>ลบหรือคืนค่าแอปพลิเคชัน

**เมื่อต้องการลบแอปพลิเคชันจากผู้เช่า Azure AD ของคุณ**:

1. ใน **พอร์ทัล Azure AD** ให้เลือก **แอปพลิเคชันขององค์กร** จากนั้นค้นหาและเลือกแอปพลิเคชันที่คุณต้องการลบ
2. **ในส่วน** จัดการ ในบานหน้าต่างด้านซ้าย **ให้เลือก** คุณสมบัติ
3. เลือก **ลบ** แล้วเลือก ใช่ **เพื่อยืนยัน** ว่าคุณต้องการลบแอปออกจากผู้เช่า Azure AD ของคุณ

For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

ใน PowerShell cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication)จะเอาการกําหนดค่าพร็อกซีแอปพลิเคชันออกจากแอปพลิเคชันที่ระบุใน Azure Active Directory และสามารถลบแอปพลิเคชันทั้งหมดถ้าระบุได้

คุณสามารถ **คืนค่าแอปพลิเคชันที่ถูกลบ** ได้โดยใช้ PowerShell เมื่อระบุแอปพลิเคชันที่คุณต้องการคืนค่าแล้ว คุณสามารถคืนค่าได้โดยใช้[Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
