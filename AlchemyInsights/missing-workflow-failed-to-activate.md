---
title: เวิร์กโฟลว์ที่หายไปไม่สามารถเปิดใช้งานได้
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065447"
---
# <a name="missing-workflow-failed-to-activate"></a>เวิร์กโฟลว์ที่หายไปไม่สามารถเปิดใช้งานได้

ในไซต์คอลเลกชัน SharePoint Microsoft คุณไม่สามารถเพิ่มเวิร์กโฟลว์ที่สามารถใช้ใหม่ได้ส่วนกลาง (เช่น "การอนุมัติ - SharePoint 2010") ลงในรายการหรือไลบรารี
  
เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้: 
  
1. เปิดเว็บไซต์รากของไซต์คอลเลกชันใน SharePoint Designer 2013
  
2. **ภายใต้ วัตถุ** ของไซต์ **ให้เลือก** เวิร์กโฟลว์ 
  
3. ในส่วน **ใหม่** ของ Ribbon **เวิร์กโฟลว์ ให้เลือก** เวิร์กโฟลว์ **ที่กลับมาใช้ใหม่** ได้ 
  
4. บนฟอร์ม **สร้างเวิร์กโฟลว์ที่กลับมาใช้** ใหม่ได้ ให้ใส่ชื่อ ** *Repair2010* ** For **Platform Type**, click SharePoint **2010 Workflow**, and then click **OK**. 
  
1. ในส่วน **บันทึก** ของ **Ribbon** เวิร์กโฟลว์ **ให้เลือก** เผยแพร่ 
  
2. ในส่วน **จัดการ** ของ **Ribbon** เวิร์กโฟลว์ **ให้เลือก ประกาศ** ส่วนกลาง ในกล่องโต้ตอบการยืนยันที่ปรากฏขึ้น **ให้เลือก** ตกลง 
  
3. ในเว็บเบราว์เซอร์ ให้ค้นหาเว็บไซต์รากของไซต์คอลเลกชัน จากนั้นเข้าถึง ไซต์ การตั้งค่า \> **ฟีเจอร์ไซต์คอลเลกชัน** จากนั้นสลับ **ฟีเจอร์เวิร์กโฟลว์** : 
  
· ถ้าฟีเจอร์  *ถูก*  เปิดใช้งาน **ให้คลิก** ปิดใช้งาน **แล้วคลิก** เปิดใช้งาน 
  
· ถ้าฟีเจอร์ *ปิดใช้งาน***ให้คลิก** เปิดใช้งาน 
  
โปรดดูข้อมูลเพิ่มเติมที่ [บทความ](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)ต่อไปนี้
  

