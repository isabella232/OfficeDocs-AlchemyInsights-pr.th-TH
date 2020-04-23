---
title: ความล่าช้าในการรับการแจ้งเตือน SharePoint และ OneDrive
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
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742020"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="ee298-102">ความล่าช้าในการรับการแจ้งเตือน SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="ee298-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="ee298-103">ตรวจสอบโฟลเดอร์ขยะหรือสแปมในอีเมลของคุณก่อน</span><span class="sxs-lookup"><span data-stu-id="ee298-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="ee298-104">ถ้า**การแจ้งเตือนทั้งหมดจากหลายแฟ้มหรือไลบรารีล่าช้า**ให้ไปที่[แดชบอร์ดของ 'สถานบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth)' เพื่อตรวจสอบคําแนะนํา/เหตุการณ์ใดๆ ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="ee298-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ee298-105">ปัญหาอาจอยู่กับความสามารถของการแจ้งเตือน SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange</span><span class="sxs-lookup"><span data-stu-id="ee298-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ee298-106">นอกจากนี้ยังทราบว่าอีเมลอื่นๆ จะถูกจัดส่ง -- ถ้าไม่ปัญหามีแนวโน้มความล่าช้าของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="ee298-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="ee298-107">ถ้า**การแจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุไม่ถูกจัดส่ง**ให้พยายามลบและสร้างใหม่</span><span class="sxs-lookup"><span data-stu-id="ee298-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="ee298-108">ดู[จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="ee298-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="ee298-109">ไม่สามารถส่งข้อความแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้</span><span class="sxs-lookup"><span data-stu-id="ee298-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="ee298-110">เฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ee298-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="ee298-111">คุณไม่สามารถกําหนดแม่แบบอีเมลการแจ้งเตือนเองได้</span><span class="sxs-lookup"><span data-stu-id="ee298-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="ee298-112">คุณต้องใช้กระแสของ Microsoft หรือเวิร์กโฟลว์ SharePoint Designer เพื่อให้บรรลุผล</span><span class="sxs-lookup"><span data-stu-id="ee298-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
