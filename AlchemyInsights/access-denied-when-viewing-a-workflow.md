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
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955220"
---
# <a name="access-denied-when-viewing-a-workflow"></a>การเข้าถึงถูกปฏิเสธเมื่อดูเวิร์กโฟลว์

SharePoint 2013 เวิร์กโฟลว์ที่พยายามส่งอีเมลไปยังกลุ่ม SharePoint อาจล้มเหลวด้วยข้อความแสดงข้อผิดพลาด "การเข้าถึงถูกปฏิเสธ" ถ้าไม่ได้ตั้งค่าการเป็นสมาชิกของกลุ่ม SharePoint เป็น ทุกคน
  
 **เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:**
  
 1. อนุญาตให้ทุกคนเห็นสมาชิกSharePointกลุ่ม
  
 2. เอากลุ่มSharePointออกจากบรรทัด ถึง หรือ ส.ค. ของอีเมล
  
 3. เพิ่มผู้ใช้ลงในบรรทัด ถึง หรือ ส.ค. ถ้าไม่สามารถเปลี่ยนแปลงการมองเห็นการเป็นสมาชิกSharePointกลุ่มได้
  
หากต้องการดูรายละเอียดเพิ่มเติม โปรดดูที่ HTTP ไม่ได้รับอนุญาตเป็น[/_vti_bin/client.svc/sp.utilities.utility.SendAmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  