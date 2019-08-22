---
title: การคืนค่ากล่องจดหมายถูกลบไปแล้ว
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.date: 2/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7b5b4e06-6943-4b2f-b8e4-cdaf13e65c77
ms.custom: ''
ms.openlocfilehash: 6ded2ad450725d9d3592c7763b24b3a211fa973e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509596"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="9abea-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="9abea-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="9abea-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="9abea-103">When a user loses their Exchange Online license, their mailbox is retained for 30 days.</span></span> <span data-ttu-id="9abea-104">ในระหว่างรอบระยะเวลา 30 วันนั้น กล่องจดหมายสามารถถูกกู้คืน โดยการกำหนดสิทธิ์การใช้งานให้กับผู้ใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="9abea-104">During that 30-day period, the mailbox can be recovered by re-assigning the license to the user.</span></span> <span data-ttu-id="9abea-105">อย่างไรก็ตาม นี้ได้เท่ากับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="9abea-105">However, this is only possible for 30 days.</span></span>
  
<span data-ttu-id="9abea-106">ในเว็บไซต์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="9abea-106">In the Admin Portal:</span></span>
  
- <span data-ttu-id="9abea-107">ไปยัง**ผู้ใช้** \> **ผู้ใช้ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="9abea-107">Go to **Users** \> **Active users**.</span></span> <span data-ttu-id="9abea-108">เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="9abea-108">Select the user in question.</span></span>

- <span data-ttu-id="9abea-109">เลือก**แก้ไข**ในการปรับเปลี่ยนสิทธิ์การใช้งานผลิตภัณฑ์</span><span class="sxs-lookup"><span data-stu-id="9abea-109">Select **Edit** to modify product licenses.</span></span>

- <span data-ttu-id="9abea-110">กำหนดสิทธิ์การใช้งานที่ออนไลน์ของ Exchange ไปยังผู้ใช้ จากนั้น**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="9abea-110">Assign the Exchange Online license to the user, and then select **Save**.</span></span>

<span data-ttu-id="9abea-111">กล่องจดหมายที่ใช้ร่วมกันจะได้รับคืนภายใน 30 วัน</span><span class="sxs-lookup"><span data-stu-id="9abea-111">Shared mailboxes are also recoverable within 30 days.</span></span> <span data-ttu-id="9abea-112">คุณสามารถค้นหาจดหมายที่ใช้ร่วมกันภายใต้**ผู้ใช้** \> **ผู้ใช้ที่ถูกลบ**ได้</span><span class="sxs-lookup"><span data-stu-id="9abea-112">You can find shared mailboxes under **Users** \> **Deleted users**.</span></span> <span data-ttu-id="9abea-113">กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="9abea-113">Shared mailboxes do not require an Exchange Online license.</span></span>
  