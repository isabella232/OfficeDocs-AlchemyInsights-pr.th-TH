---
title: ให้สิทธิ์การเข้าถึงSharePoint OneDrive
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
ms.openlocfilehash: 8c27997b1bca1d47ad876a0a6941607517912333
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58333142"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>ให้สิทธิ์การเข้าถึงSharePoint OneDrive

**หมายเหตุ**: ถ้าOneDriveหรือSharePointไซต์ของคุณไม่พร้อมใช้งานกับผู้ใช้หลายรายที่เคยเข้าถึงอาจมีปัญหาชั่วคราวของบริการ [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)
  
ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถลงชื่อเข้าใช้และใช้งาน SharePoint และ OneDrive ได้ คุณต้องเพิ่มบัญชีผู้ใช้ของพวกเขา และตรวจสอบให้แน่ใจว่า พวกเขามีสิทธิ์การใช้งานที่ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์การจัดการ Microsoft 365
  
1. ไปที่หน้า [ผู้ใช้ที่ใช้งานอยู่ ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/users)ผู้ใช้ จากนั้นคลิก **เพิ่ม** ผู้ใช้
    
2. กรอกข้อมูลของผู้ใช้ และตรวจสอบให้แน่ใจว่าภายใต้ สิทธิ์การใช้งานผลิตภัณฑ์ ได้ **มอบหมาย** สิทธิ์การใช้งานแล้ว และSharePoint **Online** ถูกเลือกไว้ 
    
โปรดทราบว่าถ้าคุณอนุญาตการแชร์ภายนอกในองค์กรของคุณ ผู้ใช้สามารถแชร์SharePointและOneDriveกับบุคคลภายนอกองค์กรได้ คุณไม่เพียงแค่ให้สิทธิ์การใช้งานกับผู้ใช้ภายนอกเหล่านี้ คุณไม่ต้องเพิ่มบัญชีให้พวกเขา เว้นแต่ว่าการแชร์จะถูกตั้งค่าเป็น "เฉพาะผู้ใช้ภายนอกที่มีอยู่เท่านั้น" ในกรณีดังกล่าว หากบุคคลดังกล่าวไม่อยู่ในไดเรกทอรีขององค์กรของคุณ คุณต้องเพิ่มบุคคลดังกล่าวเป็นผู้ใช้ภายนอกในศูนย์การจัดการ Azure AD
  

