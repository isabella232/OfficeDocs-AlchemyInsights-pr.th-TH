---
title: หนึ่งในใบรับรองบริการสหพันธรัฐภายในองค์กรของคุณจะหมดอายุ
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673516"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>หนึ่งในใบรับรองบริการสหพันธรัฐภายในองค์กรของคุณจะหมดอายุ

เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:
  
- ติดตั้งโมดูลของไดเรกทอรีที่ใช้งานอยู่ของ Microsoft Azure สำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล) เมื่อต้องการทำเช่นนี้ไปที่ [Azure Active Directory PowerShell สำหรับกราฟ ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- ทำตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" จาก AD fs เมื่อผู้ใช้ที่ติดต่อกับภายนอกลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- ทำตามขั้นตอนใน[วิธีการอัปเดตหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Microsoft ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับใบรับรองสหพันธรัฐต่ออายุให้ดูที่[การต่ออายุใบรับรองสำหรับ O365 และ AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

