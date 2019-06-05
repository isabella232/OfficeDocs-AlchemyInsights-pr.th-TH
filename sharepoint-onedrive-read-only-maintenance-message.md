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
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715090"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="051e3-102">แบบอ่านอย่างเดียวสำหรับการบำรุงรักษาข้อความเมื่อคุณพยายามที่จะใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="051e3-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="051e3-103">ผู้ใช้อาจได้รับเป็นแบบอ่านอย่างเดียวสำหรับข้อความการบำรุงรักษาเมื่อพยายามใช้ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="051e3-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="051e3-104">ตรวจสอบว่า มี การบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง<a href="https://portal.office.com/adminportal/home#/MessageCenter">ศูนย์ข้อความ</a>ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="051e3-104">Check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>.</span></span> <span data-ttu-id="051e3-105">ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า<a href="https://portal.office.com/adminportal/home#/servicehealth">ความสมบูรณ์ของบริการ</a>เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="051e3-105">Finally, ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="051e3-106">ถ้าไม่มีศูนย์กลางข้อความหรือแดชบอร์ดสุขภาพบริการได้จดบันทึกไว้ทุกสิ่งที่เกี่ยวกับการบำรุงรักษาปัจจุบันสำหรับผู้เช่าของคุณ นี้อาจเป็นเบราว์เซอร์แคการตัดสินค้าจากคลัง</span><span class="sxs-lookup"><span data-stu-id="051e3-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="051e3-107">โปรดพยายามที่จะล้างแคชเบราว์เซอร์ก่อนที่จะนำทางไปยังไซต์</span><span class="sxs-lookup"><span data-stu-id="051e3-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

  <li><span data-ttu-id="051e3-108">ในเบราว์เซอร์ Microsoft ขอบ ไป<strong>เพิ่มเติม&hellip;&gt;ตั้งค่า</strong></span><span class="sxs-lookup"><span data-stu-id="051e3-108">In the Microsoft Edge browser, go to <strong>More &hellip;&gt; Settings</strong></span></span></li>  <li><span data-ttu-id="051e3-109">ภายใต้การ<strong>เรียกดูชัดเจน</strong>เลือก<strong>เลือกสิ่งที่จะยกเลิกเลือก</strong></span><span class="sxs-lookup"><span data-stu-id="051e3-109">Under <strong>Clear browsing </strong>, select <strong>Choose what to clear</strong>.</span></span></li>  <li><span data-ttu-id="051e3-110">เลือกกล่องกาเครื่องหมายข้อมูลของเว็บไซต์ที่บันทึกไว้และคุกกี้ และเลือก<strong>ล้าง</strong></span><span class="sxs-lookup"><span data-stu-id="051e3-110">Select the Cookies and saved website data check box and select <strong>Clear</strong>.</span></span></li>  </ol>  

<span data-ttu-id="051e3-111">**หมายเหตุ**: ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่นเช่น Firefox หรือกรอบได้</span><span class="sxs-lookup"><span data-stu-id="051e3-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

