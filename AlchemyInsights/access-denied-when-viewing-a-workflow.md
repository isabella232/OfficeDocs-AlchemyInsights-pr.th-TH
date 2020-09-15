---
title: การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688821"
---
# <a name="access-denied-when-viewing-a-workflow"></a>การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์

เวิร์กโฟลว์ SharePoint ๒๐๑๓ที่พยายามส่งอีเมลไปยังกลุ่ม SharePoint สามารถล้มเหลวโดยมีข้อความแสดงข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าการเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ถูกตั้งค่าให้ทุกคน
  
 **เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:**
  
 1. อนุญาตให้ทุกคนเห็นสมาชิกของกลุ่ม SharePoint
  
 2. เอากลุ่ม SharePoint ออกจากบรรทัดถึงหรือสำเนาถึงของอีเมล
  
 3. เพิ่มผู้ใช้ลงในบรรทัดถึงหรือสำเนาถึงอย่างชัดเจนถ้าการมองเห็นเป็นสมาชิกไม่สามารถเปลี่ยนแปลงได้สำหรับกลุ่ม SharePoint
  
เมื่อต้องการดูรายละเอียดเพิ่มเติมโปรดดูที่[HTTP ที่ไม่ได้รับอนุญาตให้เข้าถึง/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  