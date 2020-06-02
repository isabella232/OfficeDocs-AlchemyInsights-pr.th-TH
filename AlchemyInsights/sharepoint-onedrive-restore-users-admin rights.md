---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511203"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความไปยัง OneDrive สําหรับไซต์ธุรกิจ

ปัญหานี้ส่วนใหญ่มักเกิดขึ้นเมื่อผู้ใช้จะถูกลบ และสร้างใหม่ ด้วยชื่อผู้ใช้หลัก (UPN) เดียวกัน บัญชีใหม่ถูกสร้างขึ้น โดยใช้ค่า PUID (รหัสเฉพาะหนังสือเดินทาง) ที่แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ผู้ใช้มี PUID ไม่ถูกต้อง สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กร Active Directory (OU) ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint แล้ว จะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้

1. เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. ถ้าคุณไม่สามารถคืนค่าผู้ใช้เดิม[Remove a user from the user info list]() 
3. หลังจากเสร็จสิ้นแล้ว คุณสามารถตรวจสอบผู้ใช้มีสิทธิ์ผู้ดูแลระบบในไซต์ OneDrive โดยทําตามขั้นตอนการเพิ่ม[ผู้ดูแลระบบสําหรับ OneDrive ของผู้ใช้](https://docs.microsoft.com/sharepoint/manage-user-profiles)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูบทความ[การทําความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
