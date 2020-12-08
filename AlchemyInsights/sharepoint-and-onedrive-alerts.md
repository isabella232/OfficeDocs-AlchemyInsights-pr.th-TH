---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: e5476f4e8462f233ff2a46832742d5a1f6e14e73
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599871"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="08360-102">ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="08360-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="08360-103">ถ้าการ **แจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการมีความล่าช้า** ให้ไปที่ [แดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth) เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="08360-103">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span>
- <span data-ttu-id="08360-104">ถ้าการ **แจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่ระบุไม่ได้รับการส่ง** ให้พยายามลบและสร้างใหม่</span><span class="sxs-lookup"><span data-stu-id="08360-104">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="08360-105">ดู [จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="08360-105">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="08360-106">ตรวจสอบโฟลเดอร์อีเมลขยะหรือสแปมในอีเมลของคุณ</span><span class="sxs-lookup"><span data-stu-id="08360-106">Check the Junk or Spam folder in your email.</span></span>

> [!NOTE]
> - <span data-ttu-id="08360-107">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้</span><span class="sxs-lookup"><span data-stu-id="08360-107">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="08360-108">เฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="08360-108">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="08360-109">คุณไม่สามารถกำหนดแม่แบบอีเมลการแจ้งเตือนเองได้</span><span class="sxs-lookup"><span data-stu-id="08360-109">You cannot customize alert email templates.</span></span> <span data-ttu-id="08360-110">คุณต้องใช้ Microsoft Flow หรือเวิร์กโฟลว์ตัวออกแบบของ SharePoint เพื่อให้บรรลุเป้าหมายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="08360-110">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
