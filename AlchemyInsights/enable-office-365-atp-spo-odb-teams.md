---
title: เปิดใช้งาน ATP 365 ของ Office สําหรับ SharePoint, OneDrive และทีม Microsoft
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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703445"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="fd466-102">เปิดใช้งานการป้องกันภัยคุกคามขั้นสูงของ Office 365 สําหรับ SharePoint แบบออนไลน์ OneDrive และทีมของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="fd466-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="fd466-103">ไปที่https://protection.office.comและลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="fd466-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="fd466-104">เลือก**สิ่งที่แนบมาที่ปลอดภัย\*\*\*\*ของนโยบาย** > **การจัดการภัยคุกคาม** > </span><span class="sxs-lookup"><span data-stu-id="fd466-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="fd466-105">เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**แล้วคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="fd466-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="fd466-106">(แนะนํา) ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแล SharePoint แบบออนไลน์ เรียกใช้ cmdlet[ชุด SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วยพารามิเตอร์**DisallowInFectedFileDownload**ตั้งค่า*เป็น true*</span><span class="sxs-lookup"><span data-stu-id="fd466-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="fd466-107">(แนะนํา) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สําหรับไฟล์ที่ตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="fd466-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="fd466-108">ATP จะ nto สแกนทุกแฟ้มเดียวใน SharePoint แบบออนไลน์, OneDrive หรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="fd466-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="fd466-109">ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้กิจกรรมร่วมกันและกิจกรรมของแขกพร้อมกับการวิเคราะห์พฤติกรรมอัจฉริยะและสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="fd466-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="fd466-110">ดู[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="fd466-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>