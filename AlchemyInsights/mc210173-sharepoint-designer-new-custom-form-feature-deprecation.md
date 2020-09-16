---
title: MC210173-SharePoint Designer ใหม่คุณลักษณะฟอร์มแบบกำหนดเองแผน
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743899"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="158e4-102">MC210173-SharePoint Designer ใหม่คุณลักษณะฟอร์มแบบกำหนดเองแผน</span><span class="sxs-lookup"><span data-stu-id="158e4-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="158e4-103">เราได้ระบุปัญหาที่ส่งผลต่อฟังก์ชันการทำงานของ SharePoint Designer สำหรับการ [สร้างฟอร์มแบบกำหนดเอง](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) ภายใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="158e4-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="158e4-104">หลังจากการตรวจสอบอย่างระมัดระวังเราได้ระบุว่าไม่มีการแก้ไขปัญหาที่ทราบแล้วสำหรับปัญหานี้และเลือกที่จะปิดใช้งานฟีเจอร์การสร้างฟอร์มแบบกำหนดเองที่มีผลบังคับใช้ในเวลา 3:00 AM UTC ในวันเสาร์, 25 เมษายน๒๐๒๐</span><span class="sxs-lookup"><span data-stu-id="158e4-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="158e4-105">การเปลี่ยนแปลงนี้ไม่มีผลกระทบต่อความสามารถในการแก้ไขฟอร์มที่สร้างไว้ก่อนหน้าหรือคุณลักษณะอื่นๆที่มีอยู่ใน SharePoint Online Designer</span><span class="sxs-lookup"><span data-stu-id="158e4-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="158e4-106">หลังจากที่ทำการเปลี่ยนแปลงนี้ผู้ใช้อาจได้รับข้อผิดพลาด: "ไม่สามารถบันทึกการเปลี่ยนแปลงรายการไปยังเซิร์ฟเวอร์ได้" เมื่อสร้างฟอร์มใหม่</span><span class="sxs-lookup"><span data-stu-id="158e4-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="158e4-107">ผู้ใช้ที่มีการใช้งาน SharePoint Designer ก่อนหน้านี้เพื่อสร้างฟอร์มแบบกำหนดเองแทนที่จะสามารถใช้ [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) เพื่อวัตถุประสงค์นี้ได้</span><span class="sxs-lookup"><span data-stu-id="158e4-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="158e4-108">PowerApps เป็นเครื่องมือที่ง่ายและมีประสิทธิภาพที่ช่วยให้ผู้ใช้สามารถดำเนินการในประสบการณ์การใช้งาน SharePoint Online ที่ทันสมัยในการสร้างและแก้ไขฟอร์มแบบกำหนดเองสำหรับรายการ SharePoint และไลบรารีเอกสารได้โดยตรงจากหน้าต่างเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="158e4-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="158e4-109">PowerApps ไม่จำเป็นต้องมีความรู้เกี่ยวกับการเขียนโค้ดแบบดั้งเดิมหรือการดาวน์โหลดแอปที่เพิ่มเติมเช่น InfoPath</span><span class="sxs-lookup"><span data-stu-id="158e4-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="158e4-110">**หมายเหตุ**: ผู้ใช้ SharePoint Online Classic จำเป็นต้องสลับไปยังประสบการณ์การใช้งานที่ทันสมัยในการเข้าถึงและใช้งาน PowerApps อย่างชั่วคราว แม้ว่าฟอร์มแบบกำหนดเองทั้งหมดที่สร้างขึ้นใน PowerApps จะสามารถเข้าถึงได้โดยผู้ใช้ที่ใช้ประสบการณ์การใช้งานแบบคลาสสิกของ SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="158e4-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
