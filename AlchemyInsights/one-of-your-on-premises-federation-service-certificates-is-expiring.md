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
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810071"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="eb7b4-102">หนึ่งในใบรับรองการบริการการติดต่อกับภายนอกภายในองค์กรของคุณใกล้หมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="eb7b4-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="eb7b4-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="eb7b4-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="eb7b4-104">ติดตั้ง Microsoft Azure Active Directory Module for Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล)</span><span class="sxs-lookup"><span data-stu-id="eb7b4-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="eb7b4-105">เมื่อต้องการดาวน์โหลด ให้ไปที่ [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="eb7b4-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="eb7b4-106">ให้ปฏิบัติตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองแบบลงนามด้วยโทเค็นของ AD FS หมดอายุแล้ว" ของข้อผิดพลาด "มีปัญหาในการเข้าถึงไซต์" จาก AD FS เมื่อผู้ใช้ภายนอกลงชื่อเข้าใช้[Microsoft 365, Azure หรือ Intuned](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="eb7b4-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="eb7b4-107">Follow the steps [in How to update or repair the settings of a fededrated domain in Microsoft 365, Azure, or Intuned](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="eb7b4-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="eb7b4-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="eb7b4-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

