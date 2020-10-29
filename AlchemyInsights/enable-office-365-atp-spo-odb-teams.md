---
title: เปิดใช้งาน Office ๓๖๕ ATP สำหรับ SharePoint, OneDrive และทีม Microsoft
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801094"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="aaea1-102">เปิดใช้งาน Microsoft Defender สำหรับ Office ๓๖๕สำหรับ SharePoint Online, OneDrive และทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="aaea1-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="aaea1-103">ไปที่ https://protection.office.com แล้วลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="aaea1-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="aaea1-104">เลือก **นโยบายการจัดการภัยคุกคาม**  >  **Policy**  >  **สิ่งที่แนบมาที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="aaea1-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="aaea1-105">เลือก **เปิดใช้งาน ATP สำหรับ SharePoint, OneDrive และทีม Microsoft** แล้วคลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="aaea1-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="aaea1-106">แนะนำ ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ที่มีการตั้งค่าพารามิเตอร์ **DisallowInfectedFileDownload** เป็น *true*</span><span class="sxs-lookup"><span data-stu-id="aaea1-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="aaea1-107">แนะนำ [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) สำหรับไฟล์ที่ตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="aaea1-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="aaea1-108">ATP จะ nto สแกนทุกไฟล์เดี่ยวใน SharePoint Online, OneDrive หรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="aaea1-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="aaea1-109">ไฟล์จะสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้การแชร์และเหตุการณ์กิจกรรมของผู้เยี่ยมชมพร้อมกับสมาร์ทวริและสัญญาณการคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="aaea1-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="aaea1-110">ให้ดูที่[ATP สำหรับ SharePoint, OneDrive และทีม Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="aaea1-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>