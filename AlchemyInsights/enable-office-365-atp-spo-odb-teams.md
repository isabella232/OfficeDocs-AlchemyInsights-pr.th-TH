---
title: เปิดใช้งาน Office 365 ATP สำหรับ SharePoint, OneDrive และทีม งานของ Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031118"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="daa91-102">เปิดใช้งานการป้องกันการคุกคามขั้นสูง 365 Office สำหรับ SharePoint แบบออนไลน์ OneDrive และทีม งานของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="daa91-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="daa91-103">ไปที่https://protection.office.comและเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="daa91-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="daa91-104">เลือก**จัดการความเสี่ยง** > **นโยบาย** > **สิ่งที่แนบมาที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="daa91-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="daa91-105">เลือก**เปิด ATP สำหรับ SharePoint, OneDrive และทีมงาน Microsoft**และจากนั้น คลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="daa91-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="daa91-106">(แนะนำ) เป็นผู้ดูแลส่วนกลางหรือผู้ดูแล SharePoint แบบออนไลน์ เรียกใช้ cmdlet[ชุด SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ที่ มีพารามิเตอร์**DisallowInfectedFileDownload**ตั้งค่าเป็น*true*</span><span class="sxs-lookup"><span data-stu-id="daa91-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="daa91-107">(แนะนำ) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สำหรับแฟ้มที่ตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="daa91-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="daa91-108">ATP จะสแกน n หากทุกแฟ้มเดียวใน SharePoint แบบออนไลน์ OneDrive หรือทีม งานของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="daa91-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="daa91-109">แฟ้มที่จะสแกนแบบอะซิงโครนัส ตลอดกระบวนการที่ใช้ร่วมกัน และบัญชี guest กิจกรรมเหตุการณ์ การศึกษาสำนึกสมาร์ทและการคุกคามสัญญาณเพื่อระบุแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="daa91-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="daa91-110">ดู[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="daa91-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>