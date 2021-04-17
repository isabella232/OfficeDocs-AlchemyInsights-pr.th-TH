---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: fd00bd90de382e325a9b8c4ce5b21d535e630730
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831249"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="0717d-102">ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="0717d-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="0717d-103">ถ้า **การแจ้งเตือนทั้งหมดจากไฟล์หรือ** ไลบรารีหลายรายการล่าช้า ให้ไปที่แดชบอร์ดสถานภาพบริการ [](https://portal.office.com/adminportal/home?ref=/servicehealth)เพื่อตรวจสอบที่ปรึกษา/เหตุการณ์ใดๆ ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="0717d-103">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span>
- <span data-ttu-id="0717d-104">**ถ้าการแจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่ระบุไม่ได้ถูกส่ง** มา พยายามลบและสร้างใหม่</span><span class="sxs-lookup"><span data-stu-id="0717d-104">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="0717d-105">ให้ดูที่ [จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="0717d-105">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="0717d-106">ตรวจสอบโฟลเดอร์อีเมลขยะหรือสแปมในอีเมลของคุณ</span><span class="sxs-lookup"><span data-stu-id="0717d-106">Check the Junk or Spam folder in your email.</span></span>

> [!NOTE]
> - <span data-ttu-id="0717d-107">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้</span><span class="sxs-lookup"><span data-stu-id="0717d-107">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="0717d-108">สนับสนุนเฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="0717d-108">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="0717d-109">คุณไม่สามารถปรับแต่งเทมเพลตอีเมลแจ้งเตือนได้</span><span class="sxs-lookup"><span data-stu-id="0717d-109">You cannot customize alert email templates.</span></span> <span data-ttu-id="0717d-110">คุณต้องใช้เวิร์กโฟลว์ Microsoft Flow หรือ SharePoint Designer เพื่อให้บรรลุเป้าหมายเหล่านั้นได้</span><span class="sxs-lookup"><span data-stu-id="0717d-110">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
