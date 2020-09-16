---
title: การแจ้งเตือนการแจ้งเตือนของ SharePoint ไม่ถูกส่ง
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751262"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="ae3df-102">การแจ้งเตือนการแจ้งเตือนของ SharePoint ไม่ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="ae3df-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="ae3df-103">โปรดตรวจสอบโฟลเดอร์อีเมลขยะในอีเมลของคุณในบางครั้งการแจ้งเตือนอาจไปที่นั่น</span><span class="sxs-lookup"><span data-stu-id="ae3df-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="ae3df-104">กำหนดว่าการ **แจ้งเตือนทั้งหมดจะไม่ถูกส่ง** หรือถ้า **การแจ้งเตือนแต่ละรายการ** จากไฟล์หรือไลบรารีที่ระบุไม่ได้ถูกส่ง</span><span class="sxs-lookup"><span data-stu-id="ae3df-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="ae3df-105">การ**แจ้งเตือนแต่ละรายการจะไม่ถูกส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนแต่ละรายการจากไฟล์หรือไลบรารีที่เฉพาะเจาะจงคุณสามารถพยายามลบและสร้างใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="ae3df-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="ae3df-106">ดู [จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="ae3df-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="ae3df-107">การ**แจ้งเตือนทั้งหมดจะไม่ถูกส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนทั้งหมดจากไฟล์หรือไลบรารีหลายรายการให้ไปที่[แดชบอร์ดสถานภาพบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคำแนะนำ/กรณีปัญหาที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="ae3df-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ae3df-108">ปัญหานี้อาจเกิดจากความสามารถในการแจ้งเตือนของ SharePoint หรือความล่าช้าในอีเมลผ่าน Exchange</span><span class="sxs-lookup"><span data-stu-id="ae3df-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ae3df-109">นอกจากนี้ยังมีความสำคัญในการสังเกตว่าอีเมลอื่นๆกำลังถูกส่งและถ้าไม่มีปัญหาเกิดขึ้นกับ Exchange ล่าช้า</span><span class="sxs-lookup"><span data-stu-id="ae3df-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="ae3df-110">คำถามที่ถามบ่อยเกี่ยวกับการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="ae3df-110">FAQ on alerts:</span></span>

- <span data-ttu-id="ae3df-111">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายเฉพาะกลุ่มความปลอดภัยและ O365 เท่านั้นที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ae3df-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="ae3df-112">คุณไม่สามารถกำหนดแม่แบบอีเมลการแจ้งเตือนเองได้ คุณจำเป็นต้องใช้เวิร์กโฟลว์ของ Microsoft FLOW หรือ SharePoint Designer เพื่อให้บรรลุเป้าหมายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="ae3df-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="ae3df-113">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="ae3df-113">Related Topics</span></span>

<span data-ttu-id="ae3df-114">ต้องการลองใช้ Microsoft Flow ใน SharePoint Online หรือไม่</span><span class="sxs-lookup"><span data-stu-id="ae3df-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="ae3df-115">สร้างขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="ae3df-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="ae3df-116">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="ae3df-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
