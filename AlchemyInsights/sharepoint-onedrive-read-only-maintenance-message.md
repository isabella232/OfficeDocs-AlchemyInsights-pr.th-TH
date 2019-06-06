---
title: การมีข้อผิดพลาด TenantAccessBlockedException เมื่อคุณเข้าถึงอีเมล 127 หรือไม่
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736421"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="4b925-102">แบบอ่านอย่างเดียวสำหรับการบำรุงรักษาข้อความเมื่อคุณพยายามที่จะใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="4b925-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="4b925-103">ผู้ใช้อาจได้รับเป็นแบบอ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="4b925-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="4b925-104">ตรวจสอบว่า มี การบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง[ศูนย์ข้อความ](https://portal.office.com/adminportal/home#/MessageCenter)ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="4b925-104">Check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="4b925-105">ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า[ความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="4b925-105">Finally, ensure you visit the[Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="4b925-106">ถ้าไม่มีศูนย์กลางข้อความหรือแดชบอร์ดสุขภาพบริการได้จดบันทึกไว้ทุกสิ่งที่เกี่ยวกับการบำรุงรักษาปัจจุบันสำหรับผู้เช่าของคุณ นี้อาจเป็นเบราว์เซอร์แคการตัดสินค้าจากคลัง</span><span class="sxs-lookup"><span data-stu-id="4b925-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="4b925-107">โปรดพยายามที่จะล้างแคชเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="4b925-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

- <span data-ttu-id="4b925-108">ในเบราว์เซอร์ Microsoft ขอบ ไปที่การตั้งค่าเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="4b925-108">In the Microsoft Edge browser, go to More  Settings</span></span>

- <span data-ttu-id="4b925-109">ภายใต้การเรียกดูชัดเจน เลือกให้เลือกสิ่งที่จะยกเลิกเลือก</span><span class="sxs-lookup"><span data-stu-id="4b925-109">Under Clear browsing, select Choose what to clear.</span></span>
- <span data-ttu-id="4b925-110">เลือกกล่องกาเครื่องหมายข้อมูลของเว็บไซต์ที่บันทึกไว้และคุกกี้ และเลือกยกเลิกการเลือก</span><span class="sxs-lookup"><span data-stu-id="4b925-110">Select the Cookies and saved website data check box and select Clear.</span></span>

<span data-ttu-id="4b925-111">**หมายเหตุ**: ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Firefox หรือกรอบได้</span><span class="sxs-lookup"><span data-stu-id="4b925-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

