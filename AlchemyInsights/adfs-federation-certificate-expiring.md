---
title: ใบรับรองสหพันธรัฐของ ADFS หมดอายุแล้ว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686773"
---
# <a name="adfs-federation-certificate-expiring"></a>ใบรับรองสหพันธรัฐของ ADFS หมดอายุแล้ว

เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:
  
1. ติดตั้งโมดูลของไดเรกทอรีที่ใช้งานอยู่ของ Microsoft Azure สำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล) เมื่อต้องการทำเช่นนี้ให้ไปที่[จัดการ AZURE AD โดยใช้ Windows PowerShell](https://aka.ms/aadposh)

2. ทำตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" จาก AD fs เมื่อผู้ใช้ที่ติดต่อกับภายนอกลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. ทำตามขั้นตอนใน[อัปเดตหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Microsoft, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับใบรับรองสหพันธรัฐต่ออายุให้ดูที่ [ต่ออายุใบรับรองของสหพันธรัฐสำหรับ Microsoft ๓๖๕และ Azure active](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)directory
