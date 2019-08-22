---
title: หนึ่งในใบรับรองของบริการสหพันธรัฐในสถานของคุณจะหมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543728"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="c1d50-102">หนึ่งในใบรับรองของบริการสหพันธรัฐในสถานของคุณจะหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="c1d50-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="c1d50-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c1d50-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="c1d50-104">ติดตั้ง Microsoft Azure ใช้งานไดเรกทอรีของโมดูลสำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลที่ไม่ได้ติดตั้งไว้แล้ว)</span><span class="sxs-lookup"><span data-stu-id="c1d50-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c1d50-105">เมื่อต้องการทำเช่นนี้ ไปที่[Azure Active Directory ของ PowerShell สำหรับกราฟ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="c1d50-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="c1d50-106">ทำตามขั้นตอนในการ "สถานการณ์สมมติ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุแล้ว" ส่วนของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ติดต่อกับภายนอกที่ลงทะเบียนใน Office 365, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="c1d50-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="c1d50-107">ทำตามขั้นตอนใน[วิธีการปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนใน Office 365, Azure หรือ Intune ที่ติดต่อกับภายนอก](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)t</span><span class="sxs-lookup"><span data-stu-id="c1d50-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="c1d50-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ดู[ต่ออายุใบรับรองสำหรับ O365 และ Azure โฆษณา](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="c1d50-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

