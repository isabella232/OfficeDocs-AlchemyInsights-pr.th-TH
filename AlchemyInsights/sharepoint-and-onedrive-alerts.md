---
title: ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563529"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="efa85-102">ความล่าช้าในการรับการแจ้งเตือนของ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="efa85-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="efa85-103">ตรวจสอบโฟลเดอร์ขยะหรือสแปมในอีเมลของคุณ</span><span class="sxs-lookup"><span data-stu-id="efa85-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="efa85-104">ถ้า**การแจ้งเตือนทั้งหมดจากหลายแฟ้มหรือไลบรารีถูกหน่วงไป**เยี่ยมชม[แดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth)เพื่อตรวจสอบคําแนะนํา/เหตุการณ์ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="efa85-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="efa85-105">ปัญหาอาจมาพร้อมกับความสามารถในการแจ้งเตือน SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange</span><span class="sxs-lookup"><span data-stu-id="efa85-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="efa85-106">นอกจากนี้โปรดทราบว่าอีเมลอื่น ๆ จะถูกจัดส่งหรือไม่</span><span class="sxs-lookup"><span data-stu-id="efa85-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="efa85-107">ถ้า**การแจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุไม่ได้ส่ง**ให้พยายามลบและสร้างใหม่</span><span class="sxs-lookup"><span data-stu-id="efa85-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="efa85-108">ดู[จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="efa85-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="efa85-109">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้</span><span class="sxs-lookup"><span data-stu-id="efa85-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="efa85-110">เฉพาะกลุ่มความปลอดภัยและ O365 ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="efa85-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="efa85-111">คุณไม่สามารถกําหนดเทมเพลตอีเมลแจ้งเตือนเองได้</span><span class="sxs-lookup"><span data-stu-id="efa85-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="efa85-112">คุณต้องใช้เวิร์กโฟลว์ Microsoft Flow หรือ SharePoint Designer เพื่อให้เวิร์กโฟลว์เหล่านั้นสําเร็จ</span><span class="sxs-lookup"><span data-stu-id="efa85-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
