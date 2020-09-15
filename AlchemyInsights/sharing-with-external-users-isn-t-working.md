---
title: การแชร์กับผู้ใช้ภายนอกไม่ทำงาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691594"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>แก้ไขปัญหาการแชร์เนื้อหา SharePoint กับผู้ใช้ภายนอก

ตรวจสอบให้แน่ใจว่ามีการเปิดใช้งานการแชร์ภายนอกสำหรับองค์กรของคุณ:
  
1. ไปที่[ &amp; หน้า Add-in ของบริการในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)แล้วคลิก**ไซต์**
    
2. ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิดใช้งาน "เปิด" ถ้ามีการเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่แล้ว" ให้ตรวจสอบให้แน่ใจว่าผู้ใช้ภายนอกแสดงอยู่ในศูนย์การจัดการ Microsoft ๓๖๕
    
ตรวจสอบให้แน่ใจว่าการแชร์ภายนอกเปิดใช้งานสำหรับไซต์แล้ว สำหรับไซต์คอลเลกชันแบบคลาสสิก:
  
1. ในศูนย์การจัดการ SharePoint ใหม่ในบานหน้าต่างด้านซ้ายให้คลิก**ไซต์**
    
2. เลือกไซต์หรือไซต์และบน ribbon ให้คลิกการ**แชร์**
    
สำหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕หรือไซต์การติดต่อสื่อสาร:
  
- ชนิดไซต์ใหม่เหล่านี้จะมีการตั้งค่าการแชร์เดียวกันกับการตั้งค่าทั้งองค์กรของคุณเว้นแต่การตั้งค่าทั้งองค์กรช่วยให้การใช้ไฟล์ร่วมกันโดยใช้ลิงก์ที่ไม่จำเป็นต้องลงชื่อเข้าใช้ ในกรณีนี้ไซต์จะอนุญาตให้มีการแชร์กับผู้ใช้ภายนอกใหม่และผู้ใช้ภายนอกที่มีอยู่แล้วในการลงชื่อเข้าใช้ เมื่อต้องการเปลี่ยนการตั้งค่าสำหรับไซต์ที่เฉพาะเจาะจงให้ใช้ศูนย์การจัดการ SharePoint ใหม่หรือ PowerShell [เรียนรู้เพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> การตั้งค่าการแชร์ภายนอกสำหรับไซต์ใดก็ได้จะเข้มงวดกว่าการตั้งค่าทั้งองค์กรของคุณแต่จะไม่ permissive มากกว่าการตั้งค่าทั้งองค์กร 
  

