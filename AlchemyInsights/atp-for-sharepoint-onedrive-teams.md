---
title: Microsoft Defender Office 365 for SharePoint, OneDrive และ Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543596"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="ff1a4-102">Microsoft Defender Office 365 for SharePoint, OneDrive และ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ff1a4-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="ff1a4-103">ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อเปิดใช้งาน Microsoft Defender Office 365:</span><span class="sxs-lookup"><span data-stu-id="ff1a4-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="ff1a4-104">ไปที่ [https://protection.office.com](https://protection.office.com) และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="ff1a4-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="ff1a4-105">ในบานหน้าต่างนําทางด้านซ้าย ภายใต้ **การจัดการภัยคุกคาม** ให้เลือก \> **นโยบายสิ่งที่แนบมา** ที่ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="ff1a4-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="ff1a4-106">เลือก **เปิด Defender Office 365 for SharePoint OneDrive, Microsoft Teams**</span><span class="sxs-lookup"><span data-stu-id="ff1a4-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="ff1a4-107">[สร้างนโยบายการแจ้งเตือนกิจกรรม](/microsoft-365/compliance/create-activity-alerts) เพื่อรับการแจ้งเตือนเมื่อเราตรวจพบไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="ff1a4-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="ff1a4-108">ดูคําแนะ[นําทั้งหมดได้ ให้ดู เปิดสิ่งที่แนบมาที่ปลอดภัยSharePoint OneDrive Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="ff1a4-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="ff1a4-109">**หมายเหตุ**: ตามการออกแบบ Microsoft Defender for Office 365จะไม่สแกนทุกไฟล์ใน SharePoint Online, OneDrive for Business หรือ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ff1a4-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="ff1a4-110">ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้กิจกรรมการแชร์ กิจกรรมของแขก และสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="ff1a4-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="ff1a4-111">ดูข้อมูลเพิ่มเติมที่[สิ่งที่แนบมาที่ปลอดภัยSharePoint OneDrive Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="ff1a4-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
