---
title: ATP สําหรับ SharePoint, วันไดรฟ์ และทีมไมโครซอฟท์
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
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508431"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="8a546-102">ATP สําหรับ SharePoint, วันไดรฟ์ และทีมไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="8a546-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="8a546-103">ทําตามขั้นตอนเหล่านี้เพื่อเปิดใช้งานการป้องกันภัยคุกคามขั้นสูง:</span><span class="sxs-lookup"><span data-stu-id="8a546-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="8a546-104">ไปที่ [https://protection.office.com](https://protection.office.com) และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือผู้ดูแลความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="8a546-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="8a546-105">ในบานหน้าต่างการนําทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**Policy** \> **สิ่งที่แนบมาที่ปลอดภัย**ของนโยบาย</span><span class="sxs-lookup"><span data-stu-id="8a546-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="8a546-106">เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**</span><span class="sxs-lookup"><span data-stu-id="8a546-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="8a546-107">[สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts)เพื่อรับการแจ้งเตือนเมื่อเราตรวจพบไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="8a546-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="8a546-108">สําหรับคําแนะนําทั้งหมด โปรดดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="8a546-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="8a546-109">**หมายเหตุ**: โดยการออกแบบ ATP ไม่สแกนทุกไฟล์เดียวใน SharePoint แบบออนไลน์, OneDrive สําหรับธุรกิจ หรือทีมของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="8a546-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="8a546-110">ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้กิจกรรมร่วมกัน กิจกรรมของผู้เยี่ยมชม และสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="8a546-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="8a546-111">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="8a546-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
