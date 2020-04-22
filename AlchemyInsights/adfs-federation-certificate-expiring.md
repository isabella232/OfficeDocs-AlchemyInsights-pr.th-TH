---
title: ใบรับรองสหพันธรัฐ ADFS หมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710426"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="c9fca-102">ใบรับรองสหพันธรัฐ ADFS หมดอายุ</span><span class="sxs-lookup"><span data-stu-id="c9fca-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="c9fca-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c9fca-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="c9fca-104">ติดตั้ง Microsoft Azure ที่ใช้งานอยู่ไดเรกทอรีโมดูสําหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลไม่ได้ติดตั้งอยู่แล้ว)</span><span class="sxs-lookup"><span data-stu-id="c9fca-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c9fca-105">เมื่อต้องการทําเช่นนี้ ไป[จัดการ Azure โฆษณา โดยใช้ Windows PowerShell](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="c9fca-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="c9fca-106">ทําตามขั้นตอนในส่วน "สถานการณ์สมมติ 1: โฆษณา FS โทเค็นเซ็นชื่อใบรับรองหมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ที่ติดต่อกับภายนอกเข้าสู่ระบบ Microsoft 365, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="c9fca-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="c9fca-107">ทําตามขั้นตอนใน[การปรับปรุง หรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Microsoft, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="c9fca-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="c9fca-108">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองสหพันธรัฐ ให้ดูที่[ต่ออายุใบรับรองสหพันธรัฐสําหรับ Microsoft 365 และ Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="c9fca-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
