---
title: การเข้าร่วม Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405670"
---
# <a name="azure-active-directory-join"></a>การเข้าร่วม Azure Active Directory

1. ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทานบทนําสู่การจัดการอุปกรณ์ใน Azure [Active Directory](/azure/active-directory/devices/overview) ที่จะแนะนําวิธีรับอุปกรณ์ภายใต้การควบคุมไปยัง Azure AD 
1. หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์เหล่านั้นลงใน Intuned คุณจะต้องตรวจสอบให้แน่ใจว่า คุณได้กําหนดค่า[Intuned](/mem/intune/enrollment/device-enrollment)และมีสิทธิ์การใช้งาน[](/mem/intune/fundamentals/licenses-assign)ก่อน
1. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้
1. เมื่อต้องการใช้การเข้าร่วม Azure AD ให้ดู[วางแผนการเข้าร่วม Azure AD](/azure/active-directory/devices/azureadjoin-plan)

For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).
