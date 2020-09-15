---
title: ใบรับรองสหพันธรัฐของ ADFS หมดอายุแล้ว
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686773"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="72cc5-102">ใบรับรองสหพันธรัฐของ ADFS หมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="72cc5-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="72cc5-103">เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="72cc5-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="72cc5-104">ติดตั้งโมดูลของไดเรกทอรีที่ใช้งานอยู่ของ Microsoft Azure สำหรับ Windows PowerShell บนคอมพิวเตอร์ (ถ้ายังไม่ได้ติดตั้งโมดูล)</span><span class="sxs-lookup"><span data-stu-id="72cc5-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="72cc5-105">เมื่อต้องการทำเช่นนี้ให้ไปที่[จัดการ AZURE AD โดยใช้ Windows PowerShell](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="72cc5-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="72cc5-106">ทำตามขั้นตอนในส่วน "สถานการณ์สมมติที่ 1: ใบรับรองการเซ็นชื่อโทเค็น FS โฆษณาที่หมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" จาก AD fs เมื่อผู้ใช้ที่ติดต่อกับภายนอกลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="72cc5-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="72cc5-107">ทำตามขั้นตอนใน[อัปเดตหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Microsoft, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="72cc5-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="72cc5-108">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับใบรับรองสหพันธรัฐต่ออายุให้ดูที่ [ต่ออายุใบรับรองของสหพันธรัฐสำหรับ Microsoft ๓๖๕และ Azure active](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)directory</span><span class="sxs-lookup"><span data-stu-id="72cc5-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
