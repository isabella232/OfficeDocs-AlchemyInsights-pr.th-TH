---
title: ใช้ร่วมกันกับผู้ใช้ภายนอกไม่ทำงาน
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207704"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>แก้ไขปัญหาเนื้อหา SharePoint การใช้ร่วมกันกับผู้ใช้ภายนอก

ตรวจสอบให้แน่ใจว่า มีการใช้ร่วมกันภายนอกเปิดอยู่สำหรับองค์กรของคุณ:
  
1. ไป[บริการ&amp;หน้าเพิ่มเติมใน Microsoft 365 admin ศูนย์](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)คลิก**ไซต์**
    
2. ตรวจสอบว่า มีเปิดการตั้งค่าการ "บน" ถ้ามีเลือก "เท่านั้นที่มีอยู่แล้วผู้ใช้ภายนอก" ต้องแน่ใจว่า ผู้ใช้ภายนอกจะอยู่ในศูนย์กลาง Microsoft 365 admin
    
ตรวจสอบว่า ภายนอกที่ใช้ร่วมกันจะเปิดใช้งานสำหรับไซต์นี้ สำหรับคลาสสิไซต์คอลเลกชัน:
  
1. ในแบบคลาสสิก SharePoint admin ศูนย์ ในบานหน้าต่างด้านซ้าย คลิก**ไซต์คอลเลกชัน**
    
2. เลือกไซต์หรือไซต์ บน ribbon คลิ ก**ใช้ร่วมกัน**
    
ไซต์สำหรับทีมที่เป็นสมาชิกของกลุ่มมี Office 365 หรือไซต์สื่อสาร:
  
- ชนิดของไซต์เหล่านี้ใหม่ได้แบบเดียวกันร่วมกันการตั้งค่าเป็นการตั้งค่าทั่วทั้งองค์กร ยกเว้นว่ามีการตั้งค่าทั่วทั้งองค์กรอนุญาตให้ใช้ร่วมกันแฟ้มโดยใช้การเชื่อมโยงที่ไม่จำเป็นต้องเข้าสู่ระบบ ในกรณีนี้ ไซต์อนุญาตให้ใช้ร่วมกับที่มีอยู่ และใหม่ภายนอกผู้ใช้ที่เข้าสู่ระบบ เมื่อต้องการเปลี่ยนการตั้งค่าสำหรับไซต์ที่เฉพาะเจาะจง ใช้ศูนย์ดูแล SharePoint ใหม่ (ตัวอย่าง) หรือ PowerShell [ศึกษาเพิ่มเติม](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> การตั้งค่าที่ใช้ร่วมกันที่ภายนอกสำหรับไซต์ใด ๆ ก็ได้เข้มงวดมากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร แต่อ่านไม่มากขึ้นกว่าการตั้งค่าทั่วทั้งองค์กร 
  

