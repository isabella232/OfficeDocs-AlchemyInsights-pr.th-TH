---
title: MC210173 - การเลิกใช้งานคุณลักษณะฟอร์มแบบกําหนดเองใหม่ของ SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928546"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="8f76c-102">MC210173 - การเลิกใช้งานคุณลักษณะฟอร์มแบบกําหนดเองใหม่ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="8f76c-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="8f76c-103">เราได้ระบุปัญหาที่มีผลต่อฟังก์ชันตัวออกแบบของ SharePoint สําหรับ[การสร้างฟอร์มแบบกําหนดเอง](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)ภายใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="8f76c-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="8f76c-104">หลังจากการตรวจสอบอย่างรอบคอบเราได้กําหนดว่ามีการแก้ไขที่ทราบกันดีสําหรับปัญหานี้และได้เลือกที่จะปิดการใช้งานคุณลักษณะการสร้างฟอร์มที่กําหนดเองที่มีประสิทธิภาพณเวลา 3:00 AM UTC ในวันเสาร์ที่ 25 เมษายน 2020</span><span class="sxs-lookup"><span data-stu-id="8f76c-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="8f76c-105">การเปลี่ยนแปลงนี้ไม่มีผลกระทบต่อความสามารถในการแก้ไขฟอร์มที่สร้างขึ้นก่อนหน้านี้หรือคุณลักษณะอื่น ๆ ที่มีอยู่ในตัวออกแบบ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="8f76c-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="8f76c-106">หลังจากที่ทําการเปลี่ยนแปลงนี้ ผู้ใช้อาจได้รับข้อผิดพลาด: "ไม่สามารถบันทึกการเปลี่ยนแปลงรายการไปยังเซิร์ฟเวอร์"</span><span class="sxs-lookup"><span data-stu-id="8f76c-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="8f76c-107">ผู้ใช้ที่เคยใช้ประโยชน์ SharePoint Designer เพื่อสร้างฟอร์มแบบกําหนดเองจะสามารถใช้[PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)สําหรับวัตถุประสงค์นี้แทน</span><span class="sxs-lookup"><span data-stu-id="8f76c-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="8f76c-108">PowerApps เป็นเครื่องมือที่ง่าย และมีประสิทธิภาพที่ช่วยให้ผู้ใช้ที่ปฏิบัติการในประสบการณ์ Modern ออนไลน์ของ SharePoint เพื่อสร้างและแก้ไขแบบกําหนดเองฟอร์มสําหรับ SharePoint รายการและไลบรารีเอกสารขวาจากหน้าต่างเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="8f76c-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="8f76c-109">PowerApps ไม่จําเป็นต้องมีความรู้การเข้ารหัสแบบดั้งเดิมหรือการดาวน์โหลดแอปเพิ่มเติมเช่น InfoPath</span><span class="sxs-lookup"><span data-stu-id="8f76c-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="8f76c-110">**หมายเหตุ**: ผู้ใช้ SharePoint Online Classic จะต้องสลับไปยังประสบการณ์สมัยใหม่ชั่วคราวเพื่อเข้าถึงและใช้ PowerApps ชั่วคราว แม้ว่า ฟอร์มแบบกําหนดเองทั้งหมดที่สร้างขึ้นใน PowerApps จะสามารถเข้าถึงได้ โดยผู้ใช้ประสบการณ์ใช้งานแบบออนไลน์ของ SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="8f76c-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
