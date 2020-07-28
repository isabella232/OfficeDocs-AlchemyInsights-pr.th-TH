---
title: ควบคุมการปรับปรุงอัตโนมัติสําหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439927"
---
# <a name="control-automatic-updates-for-office-apps"></a>ควบคุมการปรับปรุงอัตโนมัติสําหรับแอป Office

โดยค่าเริ่มต้น อย่างไรก็ตาม ผู้ดูแลระบบสามารถควบคุมวิธีการใช้การปรับปรุง โดยใช้การตั้งค่าการปรับปรุง Office การตั้งค่าการปรับปรุงช่วยให้ผู้ดูแลระบบสามารถเปิดใช้งานหรือปิดใช้งานการปรับปรุงอัตโนมัติ**Update Now** สําหรับข้อมูลโดยละเอียด โปรดดู:

- [กําหนดค่าการตั้งค่าการปรับปรุงสําหรับ Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [การปรับปรุงอัตโนมัติสําหรับ Office ไม่ได้เปิดใช้งาน](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [กําหนดวิธีการปรับปรุง Office หลังจากที่มีการติดตั้ง](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

เมื่อต้องการตรวจสอบการปรับปรุงที่มีอยู่การตั้งค่าที่ใช้กับเครื่องไคลเอ็นต์ ให้ทําตามขั้นตอนเหล่านี้:

1. เปิดตัวแก้ไขรีจิสทรี โดยไปที่**เริ่ม**  >  **เรียกใช้**  >  **regedit**
2. สลับไปยังตําแหน่งที่ตั้งต่อไปนี้ และตรวจทานการตั้งค่าการปรับปรุง Office:  
    a. HKEY_LOCAL_MACHINE\ซอฟต์แวร์\ไมโครซอฟท์\สํานักงาน\  
    b. คลิกเพื่อเรียกใช้\การกําหนดค่า

**หมายเหตุ**  ถ้าคีย์ OfficeMgmtCOM ถูกตั้งค่า ไว้ คุณอาจเห็นข้อความ "โปรแกรมปรับปรุงได้รับการจัดการโดยผู้ดูแลระบบของคุณ" ใน**Office**  >  **Office**  >  **Update** สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการการปรับปรุงแอป Microsoft 365 ด้วยตัวจัดการการตั้งค่าคอนฟิกปลายทางของ Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)  