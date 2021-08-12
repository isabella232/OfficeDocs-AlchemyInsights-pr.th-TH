---
title: การแชร์กับผู้ใช้ภายนอกไม่ใช้งานได้
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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910385"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>แก้ไขปัญหาการแชร์SharePointกับผู้ใช้ภายนอก

ตรวจสอบให้แน่ใจว่าการแชร์ภายนอกเปิดอยู่ให้กับองค์กรของคุณ ดังนี้
  
1. ไปที่หน้า [ &amp; Add-in ของบริการ ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)**แล้วคลิก** ไซต์
    
2. ตรวจสอบให้แน่ใจว่าการตั้งค่าเปิดอยู่เป็น "เปิด" ถ้าเลือก "เฉพาะผู้ใช้ภายนอกที่มีอยู่" ให้ตรวจสอบให้แน่ใจว่าผู้ใช้ภายนอกอยู่ในศูนย์การจัดการ Microsoft 365
    
ตรวจสอบให้แน่ใจว่าการแชร์ภายนอกเปิดอยู่ของไซต์นั้น For a classic site collection:
  
1. ในบานหน้าต่างSharePointใหม่ ให้คลิก ไซต์ **ในบานหน้าต่าง** ด้านซ้าย
    
2. เลือกไซต์ และบน Ribbon **ให้คลิก** การแชร์
    
For a team site that belongs to a Microsoft 365 group, or a communication site:
  
- ชนิดไซต์ใหม่เหล่านี้มีการตั้งค่าการแชร์แบบเดียวกับการตั้งค่าทั่วทั้งองค์กรของคุณ เว้นแต่ว่าการตั้งค่าทั่วทั้งองค์กรจะอนุญาตการแชร์ไฟล์โดยใช้ลิงก์ที่ไม่ต้องมีการลงชื่อเข้าใช้ ในกรณีนี้ ไซต์อนุญาตการแชร์กับผู้ใช้ภายนอกใหม่และที่มีอยู่ที่ลงชื่อเข้าใช้ เมื่อต้องการเปลี่ยนการตั้งค่าของไซต์ที่ระบุ ให้ใช้ศูนย์SharePointหรือ PowerShell ใหม่ [เรียนรู้](https://go.microsoft.com/fwlink/?linkid=871863)เพิ่มเติม
    
> [!NOTE]
> การตั้งค่าการแชร์ภายนอกของไซต์ใดๆ สามารถเข้มงวดได้มากกว่าการตั้งค่าทั่วทั้งองค์กรของคุณ แต่อาจไม่อนุญาตมากกว่าการตั้งค่าทั่วทั้งองค์กร 
  

