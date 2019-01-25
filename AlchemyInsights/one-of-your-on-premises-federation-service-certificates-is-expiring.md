---
title: หนึ่งในใบรับรองของบริการสหพันธรัฐในสถานของคุณจะหมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493280"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="f020b-102">หนึ่งในใบรับรองของบริการสหพันธรัฐในสถานของคุณจะหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="f020b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="f020b-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f020b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="f020b-p101">ติดตั้ง Microsoft Azure ใช้งานไดเรกทอรีของโมดูลสำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลที่ไม่ได้ติดตั้งไว้แล้ว) เมื่อต้องการทำเช่นนี้ ไปที่[Azure Active Directory ของ PowerShell สำหรับกราฟ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f020b-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="f020b-106">ทำตามขั้นตอนในการ "สถานการณ์สมมติ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุแล้ว" ส่วนของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ติดต่อกับภายนอกที่ลงทะเบียนใน Office 365, Azure หรือ Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="f020b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="f020b-107">ทำตามขั้นตอนใน[วิธีการปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนใน Office 365, Azure หรือ Intune ที่ติดต่อกับภายนอก](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)t</span><span class="sxs-lookup"><span data-stu-id="f020b-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="f020b-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ดู[ต่ออายุใบรับรองสำหรับ O365 และ Azure โฆษณา](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="f020b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

