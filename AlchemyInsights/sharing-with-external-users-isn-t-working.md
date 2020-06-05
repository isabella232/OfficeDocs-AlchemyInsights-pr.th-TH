---
title: การแชร์กับผู้ใช้ภายนอกไม่ทํางาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582794"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>แก้ไขปัญหาการแชร์เนื้อหา SharePoint กับผู้ใช้ภายนอก

ตรวจสอบให้แน่ใจว่าเปิดการแชร์ภายนอกสําหรับองค์กรของคุณแล้ว
  
1. ไปที่หน้า[ &amp; Add-in ของบริการในศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)แล้วคลิก**ไซต์**
    
2. ตรวจสอบให้แน่ใจว่าการตั้งค่าถูกเปิดเป็น "เปิด" ถ้าเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่" ตรวจสอบให้แน่ใจว่า ผู้ใช้ภายนอกแสดงอยู่ในศูนย์การจัดการ Microsoft 365
    
ตรวจสอบให้แน่ใจว่าเปิดการแชร์ภายนอกสําหรับไซต์ สําหรับไซต์คอลเลกชันแบบคลาสสิก:
  
1. ในศูนย์การจัดการ SharePoint ใหม่ ในบานหน้าต่างด้านซ้าย ให้คลิก**ไซต์**
    
2. เลือกไซต์หรือไซต์ และบน Ribbon ให้คลิก**การใช้ร่วมกัน**
    
สําหรับไซต์ทีมที่เป็นสมาชิกของกลุ่ม Microsoft 365 หรือไซต์การติดต่อสื่อสาร:
  
- ไซต์ชนิดใหม่เหล่านี้มีการตั้งค่าการแชร์แบบเดียวกับการตั้งค่าทั่วทั้งองค์กรของคุณ เว้นแต่การตั้งค่าทั้งองค์กรจะอนุญาตให้แชร์ไฟล์โดยใช้ลิงก์ที่ไม่จําเป็นต้องลงชื่อเข้าใช้ ในกรณีนี้ ไซต์อนุญาตให้แชร์กับผู้ใช้ภายนอกใหม่และที่มีอยู่ซึ่งลงชื่อเข้าใช้ เมื่อต้องการเปลี่ยนการตั้งค่าสําหรับไซต์เฉพาะ ให้ใช้ศูนย์การจัดการ SharePoint ใหม่หรือ PowerShell [ดูเพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> การตั้งค่าการแชร์ภายนอกสําหรับไซต์ใดๆ อาจจํากัดมากกว่าการตั้งค่าทั่วทั้งองค์กรของคุณ แต่ไม่อนุญาตมากกว่าการตั้งค่าทั่วทั้งองค์กร 
  

