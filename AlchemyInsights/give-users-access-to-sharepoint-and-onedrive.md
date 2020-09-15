---
title: ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677226"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive แก่ผู้ใช้

> [!NOTE]
> ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)
  
ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถลงชื่อเข้าใช้และใช้ SharePoint และ OneDrive คุณจำเป็นต้องเพิ่มบัญชีผู้ใช้เหล่านั้นและตรวจสอบให้แน่ใจว่ามีสิทธิ์การใช้งานที่ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์การจัดการ Microsoft ๓๖๕
  
1. ไปที่[หน้าผู้ใช้ที่ใช้งานอยู่ในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/users)แล้วคลิก**เพิ่มผู้ใช้**
    
2. กรอกข้อมูลสำหรับผู้ใช้และตรวจสอบให้แน่ใจว่าภายใต้สิทธิ์การใช้งาน **ผลิตภัณฑ์**สิทธิ์การใช้งานจะถูกกำหนดและ **SharePoint Online** ถูกเลือกไว้ 
    
โปรดทราบว่าถ้าคุณอนุญาตให้มีการแชร์ภายนอกในองค์กรของคุณผู้ใช้สามารถแชร์เนื้อหา SharePoint และ OneDrive กับบุคคลภายนอกองค์กรได้ คุณไม่จำเป็นต้องให้สิทธิ์การใช้งานผู้ใช้ภายนอกเหล่านี้ นอกจากนี้คุณยังไม่จำเป็นต้องเพิ่มบัญชีผู้ใช้เหล่านั้นเว้นแต่การแชร์ถูกตั้งค่าเป็น "เฉพาะผู้ใช้ภายนอกที่มีอยู่แล้ว" ในกรณีนี้ถ้าบุคคลนั้นไม่ได้อยู่ในไดเรกทอรีขององค์กรของคุณคุณจำเป็นต้องเพิ่มบุคคลเหล่านั้นเป็นผู้ใช้ที่เป็นผู้เยี่ยมชมในศูนย์การจัดการ AD Azure
  

