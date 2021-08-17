---
title: Azure Active Directoryเข้าร่วม
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
ms.openlocfilehash: a3815d6fcabcfe81b079657c68adb89d7be244ca128af3473c6b22c1a4f7c833
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104105"
---
# <a name="azure-active-directory-join"></a>Azure Active Directoryเข้าร่วม

1. ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน บทนําสู่การจัดการอุปกรณ์ใน[Azure Active Directory](/azure/active-directory/devices/overview)ที่จะแนะนําวิธีรับอุปกรณ์ภายใต้การควบคุมไปยัง Azure AD 
1. หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์ลงใน Intuned คุณจะต้องตรวจสอบให้แน่ใจว่า คุณได้กําหนดค่า[Intuned](/mem/intune/enrollment/device-enrollment)[และได้](/mem/intune/fundamentals/licenses-assign)ให้สิทธิ์การใช้งานก่อน
1. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้
1. เมื่อต้องการใช้งานการเข้าร่วม Azure AD ให้ดู[วางแผนการเข้าร่วม Azure AD](/azure/active-directory/devices/azureadjoin-plan)

For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).
