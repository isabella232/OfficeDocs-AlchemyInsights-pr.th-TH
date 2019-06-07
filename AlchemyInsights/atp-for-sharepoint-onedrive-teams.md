---
title: ATP สำหรับ SharePoint, OneDrive และทีม งานของ Microsoft
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765476"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a4660-102">ATP สำหรับ SharePoint, OneDrive และทีม งานของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a4660-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a4660-103">ทำตามขั้นตอนเหล่านี้เพื่อเปิดใช้งานการป้องกันการคุกคามขั้นสูง:</span><span class="sxs-lookup"><span data-stu-id="a4660-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="a4660-104">ไปที่[https://protection.office.com](https://protection.office.com)และเข้าสู่ระบบ ด้วยการดูแลส่วนกลางหรือบัญชีผู้ดูแลความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="a4660-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a4660-105">ในบานหน้าต่างนำทางด้านซ้ายภายใต้การ**บริหารความเสี่ยง**เลือก**นโยบาย** \> **สิ่งที่แนบมาที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="a4660-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a4660-106">เลือก**เปิด ATP สำหรับ SharePoint, OneDrive และทีมงานของ Microsoft**</span><span class="sxs-lookup"><span data-stu-id="a4660-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a4660-107">[สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts)จะได้รับการแจ้งเตือนเมื่อเราตรวจพบแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="a4660-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a4660-108">สำหรับคำแนะนำทั้งหมด ดู[หัวข้อ](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)นี้</span><span class="sxs-lookup"><span data-stu-id="a4660-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a4660-109">**หมายเหตุ**: โดยออกแบบ ATP ไม่สแกนแฟ้มทุกแฟ้มเดียวใน SharePoint แบบออนไลน์ OneDrive สำหรับธุรกิจ หรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="a4660-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a4660-110">แฟ้มที่สแกนแบบอะซิงโครนัส โดยโปรเซสที่ใช้ร่วมกิจกรรม กิจกรรมเป็นแขก และคุกคามสัญญาณเพื่อระบุแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="a4660-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a4660-111">สำหรับข้อมูลเพิ่มเติม ให้ดู[หัวข้อ](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)นี้</span><span class="sxs-lookup"><span data-stu-id="a4660-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
