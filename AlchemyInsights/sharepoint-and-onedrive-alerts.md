---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785684"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="723c1-102">ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="723c1-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="723c1-103">ก่อนอื่นให้ตรวจสอบโฟลเดอร์อีเมลขยะหรือสแปมในอีเมลของคุณ</span><span class="sxs-lookup"><span data-stu-id="723c1-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="723c1-104">ถ้าการ **แจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการมีความล่าช้า**ให้ไปที่ [แดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth) เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="723c1-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="723c1-105">ปัญหานี้อาจเกิดขึ้นกับความสามารถในการแจ้งเตือนของ SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange</span><span class="sxs-lookup"><span data-stu-id="723c1-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="723c1-106">โปรดสังเกตว่าจะมีการส่งอีเมลอื่นๆหรือไม่ถ้าไม่มีปัญหาเกิดขึ้นกับความล่าช้าของ Exchange</span><span class="sxs-lookup"><span data-stu-id="723c1-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="723c1-107">ถ้าการ **แจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่ระบุไม่ได้รับการส่ง**ให้พยายามลบและสร้างใหม่</span><span class="sxs-lookup"><span data-stu-id="723c1-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="723c1-108">ดู [จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="723c1-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="723c1-109">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้</span><span class="sxs-lookup"><span data-stu-id="723c1-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="723c1-110">เฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="723c1-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="723c1-111">คุณไม่สามารถกำหนดแม่แบบอีเมลการแจ้งเตือนเองได้</span><span class="sxs-lookup"><span data-stu-id="723c1-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="723c1-112">คุณต้องใช้ Microsoft Flow หรือเวิร์กโฟลว์ตัวออกแบบของ SharePoint เพื่อให้บรรลุเป้าหมายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="723c1-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
