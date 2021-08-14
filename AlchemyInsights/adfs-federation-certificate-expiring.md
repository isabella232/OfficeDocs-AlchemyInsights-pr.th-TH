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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952988"
---
# <a name="adfs-federation-certificate-expiring"></a>ใบรับรองการติดต่อกับภายนอก ADFS หมดอายุ

เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:
  
1. ติดตั้ง Microsoft Azure Active DirectoryโมดูลWindows PowerShellบนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล) เมื่อต้องการเพิ่ม ให้ไปที่ จัดการ[Azure AD โดยใช้ Windows PowerShell](https://aka.ms/aadposh)

2. ให้ปฏิบัติตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองแบบลงนามด้วยโทเค็นของ AD FS หมดอายุแล้ว" ของข้อผิดพลาด "มีปัญหาในการเข้าถึงไซต์" จาก AD FS เมื่อผู้ใช้ภายนอกลงชื่อเข้าใช้[ใน Microsoft 365, Azure หรือ Intuny](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Follow the steps in [Update or repair the settings of a fededrated domain in Microsoft, Azure, or Intuned](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองการติดต่อกับภายนอก ให้ดู ต่ออายุใบรับรองการ[ติดต่อกับภายนอกMicrosoft 365และAzure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)การติดต่อกับภายนอก
