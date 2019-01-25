---
title: สหพันธรัฐ ADFS ใบรับรองหมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493652"
---
# <a name="adfs-federation-certificate-expiring"></a>สหพันธรัฐ ADFS ใบรับรองหมดอายุ

เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:
  
1. ติดตั้ง Microsoft Azure ใช้งานไดเรกทอรีของโมดูลสำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลที่ไม่ได้ติดตั้งไว้แล้ว) เมื่อต้องการทำเช่นนี้ ไปที่[จัดการโฆษณา Azure โดยใช้ Windows PowerShell](https://aka.ms/aadposh)
    
2. ทำตามขั้นตอนในการ "สถานการณ์สมมติ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุแล้ว" ส่วนของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ติดต่อกับภายนอกที่ลงทะเบียนใน Office 365, Azure หรือ Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
3. ทำตามขั้นตอนใน[วิธีการปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนใน Office 365, Azure หรือ Intune ที่ติดต่อกับภายนอก](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
    เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ดู[ใบรับรองสหพันธรัฐต่ออายุสำหรับ Office 365 และไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
    

