---
title: ควบคุมปริมาณออนไลน์ของ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716945"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="32007-102">ควบคุมปริมาณออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="32007-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="32007-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ผู้ใช้อาจได้รับ 503 เซิร์ฟเวอร์ไม่ว่างผิดพลาดเมื่อพยายามที่จะนำทางไปยังไซต์ Sharepoint หรือ OneDrive ได้</span></span><span class="sxs-lookup"><span data-stu-id="32007-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="32007-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ข้อผิดพลาดนี้อาจมีสาเหตุจากการควบคุมภายในบริการ Sharepoint ออนไลน์ของ SharePoint ใช้การควบคุมปริมาณเพื่อรักษาประสิทธิภาพและความน่าเชื่อถือของบริการออนไลน์ของ SharePoint ขีดจำกัดการควบคุมปริมาณตัวเลข ของการดำเนินการของผู้ใช้ หรือพร้อมกันเรียก (โดยสคริปต์หรือโค้ด) เพื่อป้องกันไม่ให้เกินของทรัพยากร ถ้าได้รับควบคุมปริมาณคุณ 99% ของเวลาดังกล่าวจะ มีโค้ดแบบกำหนดเอง</span></span><span class="sxs-lookup"><span data-stu-id="32007-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="32007-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำหรับข้อมูลเพิ่มเติมในการควบคุมปริมาณให้ดู<a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid การควบคุมปริมาณ หรือถูกบล็อคใน SharePoint แบบออนไลน์</a></span></span><span class="sxs-lookup"><span data-stu-id="32007-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="32007-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ถ้าคุณเชื่อว่า ข้อผิดพลาดนี้ไม่เกี่ยวข้องกับการควบคุมปริมาณ คุณสามารถตรวจสอบถ้าไม่มีการบำรุงรักษาที่เกิดขึ้นบนผู้เช่าของคุณ โดยการนำทางไปยัง<a href="https://portal.office.com/adminportal/home#/MessageCenter">ศูนย์ข้อความ</a>ที่ใช้งานอยู่ ในตอนท้าย ให้แน่ใจว่า คุณเข้าเยี่ยมชมหน้า<a href="https://portal.office.com/adminportal/home#/servicehealth">ความสมบูรณ์ของบริการ</a>เพื่อตรวจหาใด ๆ คำแนะนำสำหรับ/ปัญหาที่อาจเกิดขึ้น</span></span><span class="sxs-lookup"><span data-stu-id="32007-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>


