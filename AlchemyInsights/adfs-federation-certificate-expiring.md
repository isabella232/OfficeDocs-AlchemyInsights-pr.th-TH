---
title: ใบรับรองการติดต่อกับภายนอก ADFS หมดอายุ
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821970"
---
# <a name="adfs-federation-certificate-expiring"></a>ใบรับรองการติดต่อกับภายนอก ADFS หมดอายุ

เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:
  
1. ติดตั้ง Microsoft Azure Active Directory Module for Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล) เมื่อต้องการเพิ่ม ให้ไปที่ จัดการ[Azure AD โดยใช้ Windows PowerShell](https://aka.ms/aadposh)

2. ให้ปฏิบัติตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองแบบลงนามด้วยโทเค็นของ AD FS หมดอายุแล้ว" ของข้อผิดพลาด "มีปัญหาในการเข้าถึงไซต์" จาก AD FS เมื่อผู้ใช้ภายนอกลงชื่อเข้าใช้[Microsoft 365, Azure หรือ Intuned](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Follow the steps in [Update or repair the settings of a fededrated domain in Microsoft, Azure, or Intuned](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองการติดต่อกับภายนอก ให้ดู[ต่ออายุใบรับรองการติดต่อกับภายนอกของ Microsoft 365 และ Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
