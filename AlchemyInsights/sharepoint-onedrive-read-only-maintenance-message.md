---
title: แบบอ่านอย่างเดียวสำหรับการบำรุงรักษาข้อความเมื่อคุณพยายามที่จะใช้ SharePoint หรือ OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840534"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="30164-102">แบบอ่านอย่างเดียวสำหรับการบำรุงรักษาข้อความเมื่อคุณพยายามที่จะใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="30164-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="30164-103">ผู้ใช้อาจได้รับข้อความ**แบบอ่านอย่างเดียวสำหรับการบำรุงรักษา**เมื่อพยายามใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="30164-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="30164-104">ถ้าเป็นเช่นนั้น ตรวจสอบถ้ามี การบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)ที่ใช้งานอยู่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="30164-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="30164-105">ทำการตรวจสอบแดชบอร์[ความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/เหตุการณ์ที่อาจจะเกิดขึ้นด้วย</span><span class="sxs-lookup"><span data-stu-id="30164-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="30164-106">ถ้าแดชบอร์ดศูนย์ข้อความหรือบริการสุขภาพไม่ได้จดบันทึกไว้ทุกสิ่งที่เกี่ยวกับการบำรุงรักษาปัจจุบันสำหรับผู้เช่าของคุณ นี้อาจเป็นเบราว์เซอร์แคการตัดสินค้าจากคลัง</span><span class="sxs-lookup"><span data-stu-id="30164-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="30164-107">โปรดพยายามที่จะล้างแคชเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="30164-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="30164-108">ในเบราว์เซอร์ของคุณ Microsoft ขอบ เลือกการ**ตั้งค่า**และจากนั้น เลือก**ความเป็นส่วนตัวและความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="30164-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="30164-109">ภายใต้การ**เรียกดูชัดเจน**เลือก**เลือกสิ่งที่จะยกเลิกเลือก**</span><span class="sxs-lookup"><span data-stu-id="30164-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="30164-110">เลือก**คุกกี้และข้อมูลเว็บไซต์ที่บันทึกไว้**และเลือก**ล้าง**</span><span class="sxs-lookup"><span data-stu-id="30164-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="30164-111">ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Mozilla Firefox หรือ Google โครเมียม</span><span class="sxs-lookup"><span data-stu-id="30164-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="30164-112">อีกทางเลือกหนึ่งจะเป็นการ เปิดไซต์ SharePoint หรือ OneDrive ของคุณในหน้าต่างแบบ InPrivate ใหม่</span><span class="sxs-lookup"><span data-stu-id="30164-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>