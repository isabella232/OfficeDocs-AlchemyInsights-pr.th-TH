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
ms.openlocfilehash: e3d645f3c45525107f42a074899a30ef26bd559e5c5657e7b8ef69d406357b32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088920"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>ให้สิทธิ์การเข้าถึงSharePoint OneDrive

> [!NOTE]
> If a OneDrive or SharePoint site is not available to multiple users who previously had access, may be a temporary service issue. [ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)
  
ถ้าคุณต้องการให้บุคคลในองค์กรของคุณสามารถลงชื่อเข้าใช้และใช้งาน SharePoint และ OneDrive ได้ คุณต้องเพิ่มบัญชีผู้ใช้ของพวกเขา และตรวจสอบให้แน่ใจว่า พวกเขามีสิทธิ์การใช้งานที่ให้สิทธิ์การเข้าถึง SharePoint และ OneDrive วิธีที่ง่ายที่สุดในการเพิ่มผู้ใช้อยู่ในศูนย์การจัดการ Microsoft 365
  
1. ไปที่หน้า [ผู้ใช้ที่ใช้งานอยู่ ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/users)ผู้ใช้ **จากนั้นคลิก เพิ่ม** ผู้ใช้
    
2. กรอกข้อมูลของผู้ใช้ และตรวจสอบให้แน่ใจว่าได้เลือก ภายใต้ สิทธิ์การใช้งานผลิตภัณฑ์ สิทธิ์การใช้งานแล้ว SharePoint **Online** 
    
โปรดทราบว่าถ้าคุณอนุญาตการแชร์ภายนอกในองค์กรของคุณ ผู้ใช้สามารถแชร์SharePointและOneDriveกับบุคคลภายนอกองค์กรได้ คุณไม่ need to give these external users licenses. คุณไม่ต้องเพิ่มบัญชีให้พวกเขา เว้นแต่ว่าการแชร์จะถูกตั้งค่าเป็น "เฉพาะผู้ใช้ภายนอกที่มีอยู่เท่านั้น" ในกรณีดังกล่าว หากบุคคลดังกล่าวไม่อยู่ในไดเรกทอรีขององค์กรของคุณ คุณต้องเพิ่มบุคคลดังกล่าวเป็นผู้ใช้ภายนอกในศูนย์การจัดการ Azure AD
  

