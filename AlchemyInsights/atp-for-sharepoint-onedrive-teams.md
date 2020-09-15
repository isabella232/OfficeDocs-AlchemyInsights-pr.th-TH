---
title: ATP สำหรับ SharePoint, OneDrive และทีม Microsoft
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715580"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="f505c-102">ATP สำหรับ SharePoint, OneDrive และทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="f505c-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="f505c-103">ทำตามขั้นตอนต่อไปนี้เพื่อเปิดใช้งานการป้องกันภัยคุกคามขั้นสูง:</span><span class="sxs-lookup"><span data-stu-id="f505c-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="f505c-104">ไปที่ [https://protection.office.com](https://protection.office.com) แล้วลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="f505c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="f505c-105">ในบานหน้าต่างนำทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**นโยบาย** \> **ที่แนบมาที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="f505c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="f505c-106">เลือก**เปิดใช้งาน ATP สำหรับ SharePoint, OneDrive และ Microsoft ทีม**</span><span class="sxs-lookup"><span data-stu-id="f505c-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="f505c-107">[สร้างนโยบายการแจ้งเตือนกิจกรรม](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) เพื่อรับการแจ้งเตือนเมื่อเราตรวจหาไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="f505c-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="f505c-108">สำหรับคำแนะนำให้เสร็จสมบูรณ์ให้ดู [หัวข้อ](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)นี้</span><span class="sxs-lookup"><span data-stu-id="f505c-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="f505c-109">**หมายเหตุ**: โดยการออกแบบ ATP จะไม่สแกนทุกไฟล์เดี่ยวใน SharePoint Online, OneDrive for Business หรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="f505c-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="f505c-110">ไฟล์จะถูกสแกนแบบอะซิงโครนัสโดยกระบวนการที่ใช้การแชร์กิจกรรมกิจกรรมของผู้เยี่ยมชมและการคุกคามสัญญาณเพื่อระบุไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="f505c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="f505c-111">สำหรับข้อมูลเพิ่มเติมให้ดู [หัวข้อ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)นี้</span><span class="sxs-lookup"><span data-stu-id="f505c-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
