---
title: ใบรับรองสหพันธรัฐ ADFS หมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737208"
---
# <a name="adfs-federation-certificate-expiring"></a>ใบรับรองสหพันธรัฐ ADFS หมดอายุ

การแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:
  
1. ติดตั้ง Microsoft Azure ไดเรกทอรีที่ใช้งานอยู่โมดูลของ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลไม่ได้ติดตั้งอยู่แล้ว) การทำเช่นนี้ไป[จัดการโฆษณา Azure โดยใช้ Windows PowerShell](https://aka.ms/aadposh)

2. ทำตามขั้นตอนใน "สถานการณ์สมมติ 1: โฆษณา FS โทเค็นการเซ็นชื่อที่หมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ที่ติดต่อกับภายนอกที่ลงทะเบียนในการ Office ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. ทำตามขั้นตอนในการ[ปรับปรุงหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Office ๓๖๕, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    หากต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองของสหพันธรัฐโปรดดู[ใบรับรองสหพันธรัฐสำหรับ Office ๓๖๕และไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
