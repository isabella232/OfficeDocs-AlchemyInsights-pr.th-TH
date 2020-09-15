---
title: อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670851"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="0dba7-102">อ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="0dba7-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="0dba7-103">ผู้ใช้อาจได้รับข้อความแบบ **อ่านอย่างเดียวสำหรับการบำรุงรักษา** เมื่อพยายามใช้ SharePoint หรือ OneDrive สำหรับสถานการณ์สมมติต่อไปนี้อย่างใดอย่างหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="0dba7-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="0dba7-104">กิจกรรมการบำรุงรักษาที่วางแผนไว้หรือที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="0dba7-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="0dba7-105">ตรวจสอบได้โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/messagecenter)</span><span class="sxs-lookup"><span data-stu-id="0dba7-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="0dba7-106">มีลำดับความสำคัญสูงเหตุการณ์บริการที่ใช้งานอยู่ที่อาจจะเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="0dba7-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="0dba7-107">ตรวจสอบคำแนะนำ/เหตุการณ์ใดก็ตามโดยการนำทางไปยัง[สถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="0dba7-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="0dba7-108">สถานการณ์สมมติการกู้คืนอัตโนมัติสำหรับการฟื้นฟูที่อาจเกิดขึ้นได้เนื่องจากเหตุการณ์ที่ไม่คาดคิดบนเซิร์ฟเวอร์ที่อาจใช้เวลาน้อยกว่า30นาทีหรือดังนั้น</span><span class="sxs-lookup"><span data-stu-id="0dba7-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="0dba7-109">ไม่มีศูนย์ข้อความหรือข้อความสถานภาพบริการสำหรับการกลับมาเล็กน้อยเหล่านี้แต่คุณควรกลับมาใช้ตามปกติในเร็วๆนี้</span><span class="sxs-lookup"><span data-stu-id="0dba7-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="0dba7-110">ในบางโอกาสที่เราสังเกตว่าหนึ่งในสามสถานการณ์ที่แสดงไว้ด้านบนได้รับการคืนค่าและบริการได้รับการคืนค่าแล้วแต่แคชเบราว์เซอร์ผู้ใช้ยังไม่ได้รับการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="0dba7-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="0dba7-111">โปรดลองล้างแคชของเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="0dba7-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="0dba7-112">ในเบราว์เซอร์ Microsoft Edge ของคุณให้เลือก**การตั้งค่า**แล้วเลือกความ**เป็นส่วนตัวและความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="0dba7-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="0dba7-113">ภายใต้**ล้างการเรียกดู**ให้เลือก**เลือกสิ่งที่ต้องการล้าง**</span><span class="sxs-lookup"><span data-stu-id="0dba7-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="0dba7-114">เลือก**คุกกี้และข้อมูลเว็บไซต์ที่บันทึกไว้**แล้วเลือก**ล้าง**</span><span class="sxs-lookup"><span data-stu-id="0dba7-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="0dba7-115">ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Mozilla Firefox หรือ Google Chrome</span><span class="sxs-lookup"><span data-stu-id="0dba7-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="0dba7-116">อีกตัวเลือกหนึ่งคือการเปิดไซต์ SharePoint หรือ OneDrive ของคุณในหน้าต่างแบบ InPrivate ใหม่</span><span class="sxs-lookup"><span data-stu-id="0dba7-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>