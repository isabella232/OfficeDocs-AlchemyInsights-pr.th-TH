---
title: การแจ้งเตือนของ SharePoint ไม่ถูกจัดส่ง
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343094"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="9b4e2-102">การแจ้งเตือนของ SharePoint ไม่ถูกจัดส่ง</span><span class="sxs-lookup"><span data-stu-id="9b4e2-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="9b4e2-103">โปรดตรวจสอบโฟลเดอร์อีเมลขยะในอีเมลของคุณเนื่องจากบางครั้งการแจ้งเตือนอาจไปที่นั่น</span><span class="sxs-lookup"><span data-stu-id="9b4e2-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="9b4e2-104">กําหนดว่าการแจ้งเตือน**ทั้งหมดจะไม่ส่ง**หรือถ้า**การแจ้งเตือนแต่ละรายการ**จากแฟ้มหรือไลบรารีที่ระบุไม่ได้ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="9b4e2-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="9b4e2-105">**การแจ้งเตือนแต่ละข้อความจะไม่ถูกส่ง**: หากการแจ้งเตือนแต่ละตัวจากแฟ้มหรือไลบรารีที่ระบุไม่ได้ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="9b4e2-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="9b4e2-106">ดู[จัดการ ดู หรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="9b4e2-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="9b4e2-107">**การแจ้งเตือนทั้งหมดจะไม่ส่ง**: ถ้าการแจ้งเตือนทั้งหมดจากหลายแฟ้มหรือไลบรารีไม่ได้ส่ง ไปที่[แดชบอร์ดของสถานบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคําแนะนํา/เหตุการณ์ใด ๆ ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="9b4e2-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="9b4e2-108">ปัญหาอาจอยู่กับความสามารถของการแจ้งเตือน SharePoint หรือความล่าช้าในอีเมลผ่านอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="9b4e2-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="9b4e2-109">นอกจากนี้ยังจะเป็นสิ่งสําคัญที่จะทราบว่าอีเมลอื่น ๆ จะถูกจัดส่งและถ้าไม่ปัญหามีแนวโน้มความล่าช้าของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="9b4e2-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="9b4e2-110">คําถามที่พบบ่อยเกี่ยวกับการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="9b4e2-110">FAQ on alerts:</span></span>

- <span data-ttu-id="9b4e2-111">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้ เฉพาะกลุ่ม Security และ O365 เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="9b4e2-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="9b4e2-112">คุณไม่สามารถกําหนดแม่แบบอีเมลการแจ้งเตือนเองได้ คุณต้องใช้กระแสของ Microsoft หรือเวิร์กโฟลว์ SharePoint Designer เพื่อให้บรรลุผลเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="9b4e2-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="9b4e2-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="9b4e2-113">Related Topics</span></span>

<span data-ttu-id="9b4e2-114">ต้องการลอง Microsoft ไหลใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="9b4e2-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="9b4e2-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="9b4e2-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="9b4e2-116">SharePoint และโฟลว์</span><span class="sxs-lookup"><span data-stu-id="9b4e2-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
