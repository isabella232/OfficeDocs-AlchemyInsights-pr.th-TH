---
title: เปิดใช้งานOffice 365 ATP SharePoint OneDrive และMicrosoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543947"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="34b2d-102">เปิดใช้งาน Microsoft Defender Office 365 for SharePoint Online, OneDrive และ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="34b2d-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="34b2d-103">ไปที่ https://protection.office.com และลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="34b2d-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="34b2d-104">เลือก **นโยบาย**  >  **การจัดการ**  >  **ภัยคุกคาม สิ่งที่แนบมา** ที่ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="34b2d-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="34b2d-105">**เลือก เปิด Defender Office 365 SharePoint OneDrive Microsoft Teams** Defender **แล้วคลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="34b2d-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="34b2d-106">(แนะนนะให้) ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วย **พารามิเตอร์ DisallowInfectedFileDownload** ที่ *ตั้งค่าเป็น true*</span><span class="sxs-lookup"><span data-stu-id="34b2d-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="34b2d-107">(แนะนนะให้) [ตั้งค่าการแจ้งเตือน](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) ไฟล์ที่ถูกตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="34b2d-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="34b2d-108">Microsoft Defender Office 365จะไม่สแกนทุกไฟล์ใน SharePoint Online, OneDrive หรือ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="34b2d-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="34b2d-109">ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้เหตุการณ์กิจกรรมการแชร์และเหตุการณ์กิจกรรมของแขก พร้อมกับพฤติกรรมที่ชาญฉลาดและภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="34b2d-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="34b2d-110">ดู[Microsoft Defender Office 365 SharePoint OneDrive Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="34b2d-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>