---
title: ๑๒๕ได้รับข้อผิดพลาดสิทธิ์การใช้งานที่ไม่ถูกต้องใน Outlook บนเว็บหรือไม่
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 825d91cd81646767b100e6fc964d7a94b8bc6879
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677478"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="7b054-102">การรับข้อผิดพลาดสิทธิ์การใช้งานที่ไม่ถูกต้องใน Outlook บนเว็บ</span><span class="sxs-lookup"><span data-stu-id="7b054-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="7b054-103">ถ้าคุณกำลังใช้ Outlook บนเว็บและคุณได้รับข้อผิดพลาดที่ **ไม่ถูกต้อง** ที่มีข้อ **ผิดพลาด X-OWA-ข้อผิดพลาด: Microsoft InvalidLicenseException**สิทธิ์การใช้งาน exchange Online ของคุณไม่ได้รับมอบหมายอย่างถูกต้องหรือมีการหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="7b054-103">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired.</span></span> <span data-ttu-id="7b054-104">ผู้ดูแลระบบของคุณสามารถมอบหมายสิทธิ์การใช้งานให้กับคุณโดยทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7b054-104">Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="7b054-105">เปิด[ศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/homepage)และภายใต้**ผู้ใช้ที่ใช้งานอยู่**ให้เลือก**แก้ไขผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="7b054-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="7b054-106">ในหน้า **แก้ไขผู้ใช้** ที่เปิดอยู่ให้เลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="7b054-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="7b054-107">ในหน้าคุณสมบัติของผู้ใช้ที่เปิดอยู่ให้คลิก**แก้ไข**สำหรับสิทธิ์การใช้งาน**ผลิตภัณฑ์**</span><span class="sxs-lookup"><span data-stu-id="7b054-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="7b054-108">ในหน้า **สิทธิ์** การใช้งานผลิตภัณฑ์ที่เปิดขึ้นให้เลือกค่า **ตำแหน่งที่ตั้ง** ที่เหมาะสมและกำหนดสิทธิ์การใช้งานที่มี Exchange Online (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียด)</span><span class="sxs-lookup"><span data-stu-id="7b054-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="7b054-109">เมื่อคุณดำเนินการเสร็จสิ้นแล้ว ให้คลิกที่ **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="7b054-109">When you're finished, click **Save**.</span></span>
