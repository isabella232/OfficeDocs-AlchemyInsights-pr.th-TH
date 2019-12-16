---
title: การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050544"
---
# <a name="access-denied-when-viewing-a-workflow"></a>การเข้าถึงถูกปฏิเสธเมื่อดูลำดับงาน

SharePoint ๒๐๑๓เวิร์กโฟลว์ที่พยายามส่งเมลไปยังกลุ่ม SharePoint สามารถล้มเหลวด้วยข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าเป็นสมาชิกของกลุ่ม SharePoint ไม่ได้ตั้งค่าให้ทุกคน
  
 **ในการแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:**
  
 1. อนุญาตให้ทุกคนดูสมาชิกของกลุ่ม SharePoint ได้
  
 2. เอากลุ่ม SharePoint ออกจากบรรทัดถึงหรือ CC ของเมล
  
 3. เพิ่มผู้ใช้ลงในบรรทัดถึงหรือสำเนาถึงอย่างชัดเจนถ้าไม่สามารถเปลี่ยนการมองเห็นเป็นสมาชิกสำหรับกลุ่ม SharePoint
  
หากต้องการดูรายละเอียดเพิ่มเติมโปรดดูที่ HTTP ที่ไม่ได้รับ[อนุญาต/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  