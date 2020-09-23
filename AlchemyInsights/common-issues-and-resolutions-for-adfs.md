---
title: ปัญหาทั่วไปและวิธีแก้ปัญหาสำหรับ ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002490"
- "4832"
ms.openlocfilehash: 3bcf65b93e5c5adbfa0ca275c69da882aa125c39
ms.sourcegitcommit: aabc5178929892d532782036bfb338b4b480d4e5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/22/2020
ms.locfileid: "48213046"
---
# <a name="common-issues-and-resolutions-for-adfs"></a><span data-ttu-id="f20b6-102">ปัญหาทั่วไปและวิธีแก้ปัญหาสำหรับ ADFS</span><span class="sxs-lookup"><span data-stu-id="f20b6-102">Common issues and resolutions for ADFS</span></span>

<span data-ttu-id="f20b6-103">การกำหนดค่าของโดเมนที่ติดต่อกับภายนอกสามารถอัปเดตได้ตามที่อธิบายไว้ในบทความฐานความรู้ของ Microsoft ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="f20b6-103">The configuration of the federated domain can be updated as described in the following Microsoft Knowledge Base articles.</span></span>

- [<span data-ttu-id="f20b6-104">ใบรับรองสหพันธรัฐของ ADFS หมดอายุแล้ว</span><span class="sxs-lookup"><span data-stu-id="f20b6-104">ADFS Federation Certificate Expiring</span></span>](adfs-federation-certificate-expiring.md)

- [<span data-ttu-id="f20b6-105">ตั้งค่า ADFS สำหรับ Office ๓๖๕สำหรับการลงชื่อเข้าระบบครั้งเดียว</span><span class="sxs-lookup"><span data-stu-id="f20b6-105">Set up ADFS for Office 365 for Single Sign-On</span></span>](https://docs.microsoft.com/office365/troubleshoot/active-directory/set-up-adfs-for-single-sign-on)

- <span data-ttu-id="f20b6-106">[๒๗๑๓๘๙๘](https://support.microsoft.com/help/2713898)  "มีปัญหาเกิดขึ้นในการเข้าถึงไซต์" จาก AD fs เมื่อผู้ใช้ที่ติดต่อกับภายนอกลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="f20b6-106">[2713898](https://support.microsoft.com/help/2713898)  "There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune.</span></span>

- <span data-ttu-id="f20b6-107">[๒๕๓๕๑๙๑](https://support.microsoft.com/help/2535191) "ขออภัยแต่เรากำลังมีปัญหาในการลงชื่อเข้าใช้คุณ" และ "๘๐๐๔๘๑๖๓" ข้อผิดพลาดเมื่อผู้ใช้ที่ติดต่อกับภายนอกพยายามลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="f20b6-107">[2535191](https://support.microsoft.com/help/2535191) "Sorry, but we're having trouble signing you in" and "80048163" error when a federated user tries to sign in to Microsoft 365, Azure, or Intune.</span></span>

- <span data-ttu-id="f20b6-108">[๒๖๔๗๐๒๐](https://support.microsoft.com/help/2647020)   "ขออภัยแต่เรากำลังมีปัญหาในการลงชื่อเข้าใช้คุณ" และ "๘๐๐๔๑๓๑๗" หรือ "๘๐๐๔๓๔๓๑" เมื่อผู้ใช้ที่ติดต่อกับภายนอกพยายามลงชื่อเข้าใช้ Microsoft ๓๖๕, Azure หรือ Intune</span><span class="sxs-lookup"><span data-stu-id="f20b6-108">[2647020](https://support.microsoft.com/help/2647020)   "Sorry, but we're having trouble signing you in" and "80041317" or "80043431" error when a federated user tries to sign in to Microsoft 365, Azure, or Intune.</span></span>

<span data-ttu-id="f20b6-109">สำหรับข้อมูลเพิ่มเติมให้ดู[อัปเดตหรือซ่อมแซมการตั้งค่าของโดเมนที่ติดต่อกับภายนอกใน Microsoft ๓๖๕, Azure หรือ Intune](https://docs.microsoft.com/office365/troubleshoot/active-directory/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="f20b6-109">For more information, see [Update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/active-directory/update-federated-domain-office-365).</span></span>
