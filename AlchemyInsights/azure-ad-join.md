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
ms.openlocfilehash: 9e08d6c2a4553e395b5206816f29471118bb3b286e669c0b2d07a740e2a3c749
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894570"
---
# <a name="azure-active-directory-join"></a>Azure Active Directoryเข้าร่วม

1. ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน บทนําสู่การจัดการอุปกรณ์ใน[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview)ที่จะแนะนําวิธีรับอุปกรณ์ภายใต้การควบคุมไปยัง Azure AD 
1. หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์ลงใน Intuned คุณจะต้องตรวจสอบให้แน่ใจว่าคุณได้กําหนดค่า[Intuned](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)[และได้](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)ให้สิทธิ์การใช้งานก่อน
1. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้
1. เมื่อต้องการใช้งานการเข้าร่วม Azure AD ให้ดู[วางแผนการเข้าร่วม Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq) and for Windows 10 pro device, see [unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).
