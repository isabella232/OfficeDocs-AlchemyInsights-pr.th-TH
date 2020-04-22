---
title: หนึ่งในใบรับรองบริการสหพันธรัฐในสถานที่ของคุณกําลังจะหมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761402"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="21f84-102">หนึ่งในใบรับรองบริการสหพันธรัฐในสถานที่ของคุณกําลังจะหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="21f84-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="21f84-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="21f84-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="21f84-104">ติดตั้ง Microsoft Azure ที่ใช้งานอยู่ไดเรกทอรีโมดูสําหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลไม่ได้ติดตั้งอยู่แล้ว)</span><span class="sxs-lookup"><span data-stu-id="21f84-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="21f84-105">เมื่อต้องการทําเช่นนี้ ไปที่[Azure ที่ใช้งานอยู่ไดเรกทอรี PowerShell สําหรับกราฟ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="21f84-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="21f84-106">ทําตามขั้นตอนในส่วน "สถานการณ์สมมติ 1: โฆษณา FS โทเค็นเซ็นชื่อใบรับรองหมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ federated เข้าสู่ระบบใน Office 365, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="21f84-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="21f84-107">ทําตามขั้นตอนใน t[วิธีการปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนติดต่อกับภายนอกใน Office 365, Azure หรือ Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="21f84-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="21f84-108">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ให้ดูที่[การต่ออายุใบรับรองสําหรับ O365 และ Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="21f84-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

