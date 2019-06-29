---
title: 126 การรับกล่องจดหมายไม่พบข้อผิดพลาดใน OWA หรือไม่
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: cb26898269888183262618e20e10366c80f41c42
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35386932"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="0a64d-102">การเรียกดูกล่องจดหมายไม่พบข้อผิดพลาดใน Outlook บนเว็บหรือไม่</span><span class="sxs-lookup"><span data-stu-id="0a64d-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="0a64d-103">ถ้าคุณกำลังใช้ Outlook บนเว็บ และคุณได้รับข้อผิดพลาดที่**ไม่สามารถพบกล่องจดหมายสำหรับ**บัญชีที่คุณใช้เพื่อเชื่อมต่อกับ Outlook บนเว็บ ไม่มีสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ และดังนั้น ไม่มีกล่องจดหมายถูกเชื่อมโยงกับลูกค้าองค์กร</span><span class="sxs-lookup"><span data-stu-id="0a64d-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="0a64d-104">ผู้ดูแลระบบของคุณสามารถกำหนดสิทธิ์การใช้งานบัญชีของคุณ โดยทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="0a64d-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="0a64d-105">เปิด[Microsoft 365 admin ศูนย์](https://portal.office.com/adminportal/home#/homepage)และ**ผู้ใช้ที่ใช้งานอยู่**ใต้**แก้ไขผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="0a64d-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="0a64d-106">ใน**การแก้ไขผู้ใช้**เพจที่เปิด เลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="0a64d-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="0a64d-107">ในหน้าคุณสมบัติของผู้ใช้ที่เปิด คลิก**แก้ไข**สำหรับ**สิทธิ์การใช้งานผลิตภัณฑ์**</span><span class="sxs-lookup"><span data-stu-id="0a64d-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="0a64d-108">ในเพจ**สิทธิ์การใช้งานผลิตภัณฑ์**ที่เปิด เลือกค่า**ตำแหน่งที่ตั้ง**ที่เหมาะสม และกำหนดสิทธิ์การใช้งานที่ประกอบด้วยการแลกเปลี่ยนแบบออนไลน์ (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียดของ)</span><span class="sxs-lookup"><span data-stu-id="0a64d-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="0a64d-109">เมื่อคุณดำเนินการเสร็จสิ้นแล้ว ให้คลิกที่ **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="0a64d-109">When you're finished, click **Save**.</span></span>
