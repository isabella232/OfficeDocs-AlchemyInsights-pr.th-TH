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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620742"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="a5205-102">แบบอ่านอย่างเดียวสำหรับการบำรุงรักษาข้อความเมื่อคุณพยายามที่จะใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="a5205-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="a5205-103">ผู้ใช้อาจได้รับข้อความ**แบบอ่านอย่างเดียวสำหรับการบำรุงรักษา**เมื่อพยายามใช้ SharePoint หรือ OneDrive สำหรับหนึ่งในสถานการณ์ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a5205-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="a5205-104">กิจกรรมการบำรุงรักษาที่วางแผนไว้ หรือที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="a5205-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="a5205-105">ตรวจสอบได้ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/messagecenter)</span><span class="sxs-lookup"><span data-stu-id="a5205-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="a5205-106">เหตุการณ์บริการที่ใช้งานสูงระดับความสำคัญ ที่อาจจะเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="a5205-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="a5205-107">การตรวจสอบสำหรับคำแนะนำสำหรับ/เหตุการณ์ใด ๆ โดยการนำทางเพื่อ[ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a5205-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="a5205-108">รองซ่อมแซมอัตโนมัติกู้คืนสถานการณ์สมมติที่อาจเกิดขึ้นเนื่องจากเหตุการณ์ใด ๆ ที่ไม่คาดคิดบนเซิร์ฟเวอร์ซึ่งอาจล่าสุดที่น้อยกว่า 30 นาทีหรือดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="a5205-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="a5205-109">มีศูนย์ไม่มีข้อความ หรือบริการสุขภาพที่ลงรายการบัญชีสำหรับ recoveries เหล่านี้เล็กน้อย แต่คุณควรจะกลับสู่ปกติในไม่ช้ามาก</span><span class="sxs-lookup"><span data-stu-id="a5205-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="a5205-110">ในโอกาสไม่มาก เราได้จากสังเกตว่า หนึ่งสถานการณ์สามรายการข้างต้นมีสาเหตุ และคืนค่าบริการแล้ว แต่แคชของเบราว์เซอร์ผู้ใช้ยังไม่ถูกยกเลิกเลือกค่า</span><span class="sxs-lookup"><span data-stu-id="a5205-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="a5205-111">โปรดพยายามที่จะล้างแคชเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="a5205-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="a5205-112">ในเบราว์เซอร์ของคุณ Microsoft ขอบ เลือกการ**ตั้งค่า**และจากนั้น เลือก**ความเป็นส่วนตัวและความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="a5205-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="a5205-113">ภายใต้การ**เรียกดูชัดเจน**เลือก**เลือกสิ่งที่จะยกเลิกเลือก**</span><span class="sxs-lookup"><span data-stu-id="a5205-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="a5205-114">เลือก**คุกกี้และข้อมูลเว็บไซต์ที่บันทึกไว้**และเลือก**ล้าง**</span><span class="sxs-lookup"><span data-stu-id="a5205-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="a5205-115">ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Mozilla Firefox หรือ Google โครเมียม</span><span class="sxs-lookup"><span data-stu-id="a5205-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="a5205-116">อีกทางเลือกหนึ่งจะเป็นการ เปิดไซต์ SharePoint หรือ OneDrive ของคุณในหน้าต่างแบบ InPrivate ใหม่</span><span class="sxs-lookup"><span data-stu-id="a5205-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>