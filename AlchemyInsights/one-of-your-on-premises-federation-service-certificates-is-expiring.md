---
title: หนึ่งในใบรับรองการบริการการติดต่อกับภายนอกภายในองค์กรของคุณใกล้หมดอายุแล้ว
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985236"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>หนึ่งในใบรับรองการบริการการติดต่อกับภายนอกภายในองค์กรของคุณใกล้หมดอายุแล้ว

เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:
  
- ติดตั้ง Microsoft Azure Active DirectoryโมดูลWindows PowerShellบนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล) เมื่อต้องการเพิ่ม ให้ไปที่ Azure Active Directory [PowerShell Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- ให้ปฏิบัติตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองแบบลงนามด้วยโทเค็นของ AD FS หมดอายุแล้ว" ของข้อผิดพลาด "มีปัญหาในการเข้าถึงไซต์" จาก AD FS เมื่อผู้ใช้ภายนอกลงชื่อเข้าใช้[ใน Microsoft 365, Azure หรือ Intuny](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Follow the steps [in How to update or repair the settings of a fededrated domain in Microsoft 365, Azure, or Intuned](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

