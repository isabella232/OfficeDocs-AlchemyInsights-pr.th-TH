---
title: ใบรับรองสหพันธรัฐ ADFS หมดอายุ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737208"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="808a7-102">ใบรับรองสหพันธรัฐ ADFS หมดอายุ</span><span class="sxs-lookup"><span data-stu-id="808a7-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="808a7-103">การแก้ไขปัญหานี้ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="808a7-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="808a7-104">ติดตั้ง Microsoft Azure ไดเรกทอรีที่ใช้งานอยู่โมดูลของ Windows PowerShell บนคอมพิวเตอร์ (ถ้าโมดูลไม่ได้ติดตั้งอยู่แล้ว)</span><span class="sxs-lookup"><span data-stu-id="808a7-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="808a7-105">การทำเช่นนี้ไป[จัดการโฆษณา Azure โดยใช้ Windows PowerShell](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="808a7-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="808a7-106">ทำตามขั้นตอนใน "สถานการณ์สมมติ 1: โฆษณา FS โทเค็นการเซ็นชื่อที่หมดอายุ" ของ["มีปัญหาในการเข้าถึงไซต์" ข้อผิดพลาดจาก FS โฆษณาเมื่อผู้ใช้ที่ติดต่อกับภายนอกที่ลงทะเบียนในการ Office ๓๖๕, Azure หรือ Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="808a7-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="808a7-107">ทำตามขั้นตอนในการ[ปรับปรุงหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Office ๓๖๕, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="808a7-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="808a7-108">หากต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการต่ออายุใบรับรองของสหพันธรัฐโปรดดู[ใบรับรองสหพันธรัฐสำหรับ Office ๓๖๕และไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="808a7-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
