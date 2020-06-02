---
title: เปิดใช้งาน ATP ของ Office 365 สําหรับ SharePoint, OneDrive และทีม Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506937"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3bec3-102">เปิดใช้งานการป้องกันภัยคุกคามขั้นสูงของ Office 365 สําหรับ SharePoint แบบออนไลน์, OneDrive และทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="3bec3-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="3bec3-103">ไปที่ https://protection.office.com และลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="3bec3-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="3bec3-104">เลือก**นโยบายการจัดการภัยคุกคาม**  >  **Policy**  >  **สิ่งที่แนบมาที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="3bec3-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="3bec3-105">เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**แล้วคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="3bec3-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="3bec3-106">(แนะนํา) ในฐานะผู้ดูแลส่วนกลางหรือผู้ดูแล SharePoint Online เรียกใช้ cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วยการตั้งค่าพารามิเตอร์**DisallowInfectedFileDownload**เป็น*true*</span><span class="sxs-lookup"><span data-stu-id="3bec3-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="3bec3-107">(แนะนํา) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สําหรับแฟ้มที่ตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="3bec3-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="3bec3-108">ATP จะสแกนทุกแฟ้มเดียวใน SharePoint แบบออนไลน์, OneDrive หรือ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3bec3-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="3bec3-109">ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้กิจกรรมร่วมกันและกิจกรรมของแขกพร้อมกับ heuristics สมาร์ทและสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="3bec3-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="3bec3-110">ดู[ATP สําหรับ SharePoint, OneDrive และทีม Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="3bec3-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>