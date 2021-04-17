---
title: MC210173 - การเลิกใช้ฟีเจอร์ฟอร์มแบบปรับแต่งเองของ SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831825"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="8857d-102">MC210173 - การเลิกใช้ฟีเจอร์ฟอร์มแบบปรับแต่งเองของ SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="8857d-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="8857d-103">เราได้ระบุปัญหาที่มีผลกระทบต่อฟังก์ชันการใช้ฟังก์ชัน SharePoint Designer ในการสร้าง [ฟอร์มแบบปรับแต่งเอง](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) ภายใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8857d-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="8857d-104">หลังจากระมัดระวังการใช้ความระมัดระวัง เราได้กําหนดว่า ไม่มีการแก้ไขที่ทราบแล้วของปัญหานี้ และได้เลือกที่จะปิดใช้งานฟีเจอร์การสร้างฟอร์มแบบกําหนดเองได้อย่างมีประสิทธิภาพตั้งแต่ 3:00 น. UTC ในวันเสาร์ 25 เมษายน 2020</span><span class="sxs-lookup"><span data-stu-id="8857d-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="8857d-105">การเปลี่ยนแปลงนี้จะไม่ส่งผลกระทบต่อความสามารถในการแก้ไขฟอร์มที่สร้างไว้ก่อนหน้านี้หรือฟีเจอร์ที่มีอยู่อื่นๆ ใน SharePoint Online Designer</span><span class="sxs-lookup"><span data-stu-id="8857d-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="8857d-106">หลังจากการเปลี่ยนแปลงนี้แล้ว ผู้ใช้อาจได้รับข้อผิดพลาด: "ไม่สามารถบันทึกการเปลี่ยนแปลงรายการไปยังเซิร์ฟเวอร์ได้" เมื่อสร้างฟอร์มใหม่</span><span class="sxs-lookup"><span data-stu-id="8857d-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="8857d-107">ผู้ใช้ที่ใช้ SharePoint Designer มาก่อนหน้านี้เพื่อสร้างฟอร์มแบบปรับแต่งเองจะสามารถใช้ [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) เพื่อจุดประสงค์นี้แทนได้</span><span class="sxs-lookup"><span data-stu-id="8857d-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="8857d-108">PowerApps เป็นเครื่องมือที่ง่ายและมีประสิทธิภาพที่ช่วยให้ผู้ใช้สามารถดําเนินการในประสบการณ์ที่ทันสมัยของ SharePoint Online เพื่อสร้างและแก้ไขฟอร์มแบบปรับแต่งเองในรายการ SharePoint และไลบรารีเอกสารได้จากหน้าต่างเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="8857d-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="8857d-109">PowerApps ไม่ต้องมีการเขียนโค้ดความรู้แบบดั้งเดิมหรือการดาวน์โหลดแอปเพิ่มเติมใดๆ เช่น InfoPath</span><span class="sxs-lookup"><span data-stu-id="8857d-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="8857d-110">**หมายเหตุ**: ผู้ใช้ SharePoint Online Classic จะต้องสลับไปยังประสบการณ์การใช้งานที่ทันสมัยชั่วคราวเพื่อเข้าถึงและใช้ PowerApps แม้ว่า ฟอร์มแบบปรับแต่งเองทั้งหมดที่สร้างขึ้นใน PowerApps จะสามารถเข้าถึงได้โดยผู้ใช้ประสบการณ์การใช้งาน SharePoint Online แบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="8857d-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
