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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="ccfc8-102">ใบรับรองการติดต่อกับภายนอก ADFS หมดอายุ</span><span class="sxs-lookup"><span data-stu-id="ccfc8-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="ccfc8-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="ccfc8-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="ccfc8-104">ติดตั้ง Microsoft Azure Active Directory Module for Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล)</span><span class="sxs-lookup"><span data-stu-id="ccfc8-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="ccfc8-105">เมื่อต้องการเพิ่ม ให้ไปที่ จัดการ[Azure AD โดยใช้ Windows PowerShell](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="ccfc8-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="ccfc8-106">ให้ปฏิบัติตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองแบบลงนามด้วยโทเค็นของ AD FS หมดอายุแล้ว" ของข้อผิดพลาด "มีปัญหาในการเข้าถึงไซต์" จาก AD FS เมื่อผู้ใช้ภายนอกลงชื่อเข้าใช้[Microsoft 365, Azure หรือ Intuned](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="ccfc8-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="ccfc8-107">Follow the steps in [Update or repair the settings of a fededrated domain in Microsoft, Azure, or Intuned](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="ccfc8-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="ccfc8-108">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองการติดต่อกับภายนอก ให้ดู[ต่ออายุใบรับรองการติดต่อกับภายนอกของ Microsoft 365 และ Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="ccfc8-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
