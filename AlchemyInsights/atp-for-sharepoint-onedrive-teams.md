---
title: ATP สําหรับทีม SharePoint, OneDrive และไมโครซอฟท์
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712477"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="d5a7b-102">ATP สําหรับทีม SharePoint, OneDrive และไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="d5a7b-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="d5a7b-103">ทําตามขั้นตอนเหล่านี้เพื่อเปิดใช้งานการป้องกันภัยคุกคามขั้นสูง:</span><span class="sxs-lookup"><span data-stu-id="d5a7b-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="d5a7b-104">ไปที่[https://protection.office.com](https://protection.office.com)และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="d5a7b-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="d5a7b-105">ในบานหน้าต่างนําทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**สิ่งที่แนบที่ปลอดภัย\*\*\*\*ของนโยบาย**\></span><span class="sxs-lookup"><span data-stu-id="d5a7b-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="d5a7b-106">เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ Microsoft Teams**</span><span class="sxs-lookup"><span data-stu-id="d5a7b-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="d5a7b-107">[สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts)เพื่อรับการแจ้งเตือนเมื่อเราตรวจพบไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="d5a7b-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="d5a7b-108">สําหรับคําแนะนําทั้งหมด ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="d5a7b-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="d5a7b-109">**หมายเหตุ**: โดยการออกแบบ ATP ไม่สแกนทุกแฟ้มเดียวใน SharePoint แบบออนไลน์ OneDrive สําหรับธุรกิจ หรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="d5a7b-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="d5a7b-110">ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้กิจกรรมการแชร์ กิจกรรมของแขก และสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="d5a7b-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="d5a7b-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="d5a7b-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
