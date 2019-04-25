---
title: สหพันธรัฐ ADFS ใบรับรองหมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398359"
---
# <a name="adfs-federation-certificate-expiring"></a>สหพันธรัฐ ADFS ใบรับรองหมดอายุ

เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:
  
1. ติดตั้ง Microsoft Azure ใช้งานไดเรกทอรีของโมดูลสำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลที่ไม่ได้ติดตั้งไว้แล้ว) เมื่อต้องการทำเช่นนี้ ไปที่[จัดการโฆษณา Azure โดยใช้ Windows PowerShell](https://aka.ms/aadposh)
    
2. ทำตามขั้นตอนในการ "สถานการณ์สมมติ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุแล้ว" ส่วนของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ติดต่อกับภายนอกที่ลงทะเบียนใน Office 365, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
3. ทำตามขั้นตอนใน[วิธีการปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนใน Office 365, Azure หรือ Intune ที่ติดต่อกับภายนอก](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
    เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ดู[ใบรับรองสหพันธรัฐต่ออายุสำหรับ Office 365 และไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
    

