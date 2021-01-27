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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015020"
---
# <a name="delete-or-restore-applications"></a>ลบหรือคืนค่าแอปพลิเคชัน

**เมื่อต้องการลบแอปพลิเคชันจากผู้เช่า AZURE AD ของคุณ**:

1. ใน **พอร์ทัล AD Azure** ให้เลือก **แอปพลิเคชันสำหรับองค์กร** จากนั้นค้นหาและเลือกแอปพลิเคชันที่คุณต้องการลบ
2. ในส่วน **จัดการ** ในบานหน้าต่างด้านซ้ายให้เลือก **คุณสมบัติ**
3. เลือก **ลบ** จากนั้นเลือก **ใช่** เพื่อยืนยันว่าคุณต้องการลบแอปจากผู้เช่า Azure AD ของคุณ

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการลบแอปให้ดูที่[Quickstart: ลบแอปพลิเคชันจากผู้เช่า Azure Active directory (AZURE AD) ของคุณ](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

ใน PowerShell cmdlet การ [เอา AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) เอาการกำหนดค่าพร็อกซีของแอปพลิเคชันออกจากแอปพลิเคชันที่เฉพาะเจาะจงใน Azure active directory และสามารถลบแอปพลิเคชันทั้งหมดได้ถ้ามีการระบุไว้

คุณสามารถ **คืนค่าแอปพลิเคชันที่ถูกลบ** โดยใช้ PowerShell ได้ เมื่อแอปพลิเคชันที่คุณต้องการคืนค่าได้รับการระบุแล้วคุณสามารถคืนค่าได้โดยใช้การ[คืนค่า-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
