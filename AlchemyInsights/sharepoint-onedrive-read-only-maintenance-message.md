---
title: อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามที่จะใช้ SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051300"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="a1f07-102">อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามที่จะใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="a1f07-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="a1f07-103">ผู้ใช้อาจได้รับแบบ**อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษา**เมื่อพยายามที่จะใช้ SharePoint หรือ OneDrive สำหรับหนึ่งในสถานการณ์ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a1f07-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="a1f07-104">กิจกรรมการบำรุงรักษาที่วางแผนไว้หรือที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="a1f07-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="a1f07-105">ตรวจสอบหาพวกเขาโดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/messagecenter)</span><span class="sxs-lookup"><span data-stu-id="a1f07-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="a1f07-106">เหตุการณ์ที่มีความสำคัญสูงและการบริการที่ใช้งานอยู่ที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="a1f07-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="a1f07-107">ตรวจสอบการแนะนำ/เหตุการณ์โดยการนำทางไปยัง[บริการสุขภาพ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a1f07-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="a1f07-108">สถานการณ์จำลองการกู้คืนอัตโนมัติเล็กน้อยที่อาจเกิดขึ้นเนื่องจากเหตุการณ์ที่ไม่คาดคิดใดๆบนเซิร์ฟเวอร์ซึ่งอาจมีอายุการใช้งานน้อยกว่า30นาทีหรือมากกว่านั้น</span><span class="sxs-lookup"><span data-stu-id="a1f07-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="a1f07-109">ไม่มีศูนย์ข้อความหรือโพสต์สุขภาพบริการสำหรับการกู้คืนเล็กน้อยเหล่านี้แต่คุณควรจะกลับมาเป็นปกติเร็วๆนี้.</span><span class="sxs-lookup"><span data-stu-id="a1f07-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="a1f07-110">ในโอกาสน้อยมากที่เราสังเกตเห็นว่าหนึ่งในสามสถานการณ์ที่ระบุไว้ข้างต้นได้รับสาเหตุและการบริการได้รับการคืนค่าแต่แคชเบราว์เซอร์ผู้ใช้ไม่ได้ถูกล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="a1f07-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="a1f07-111">โปรดพยายามล้างแคชเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="a1f07-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="a1f07-112">ในเบราว์เซอร์ Microsoft Edge ของคุณให้เลือก**การตั้งค่า**แล้วเลือก**ความเป็นส่วนตัวและความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="a1f07-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="a1f07-113">ในส่วน "**ล้างการเรียกดู**" ให้เลือก**เลือกสิ่งที่ต้องการล้าง**</span><span class="sxs-lookup"><span data-stu-id="a1f07-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="a1f07-114">เลือก**คุกกี้และข้อมูลเว็บไซต์ที่บันทึกไว้**แล้วเลือก "**ล้าง**"</span><span class="sxs-lookup"><span data-stu-id="a1f07-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="a1f07-115">ขั้นตอนเหล่านี้อาจแตกต่างกันไปเมื่อใช้เบราว์เซอร์อื่นๆเช่น Mozilla Firefox หรือ Google โครเมียม</span><span class="sxs-lookup"><span data-stu-id="a1f07-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="a1f07-116">ตัวเลือกอื่นจะเปิดไซต์ SharePoint ของคุณหรือ OneDrive ในหน้าต่างแบบ InPrivate ใหม่</span><span class="sxs-lookup"><span data-stu-id="a1f07-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>