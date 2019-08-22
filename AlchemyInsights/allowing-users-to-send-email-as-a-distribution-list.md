---
title: 717 Allowing ให้ผู้ใช้ส่งอีเมลที่เป็นรายการการแจกจ่าย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/13/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "717"
- "3"
ms.assetid: d9e5f5be-b653-44a9-bce8-9ca11396d39e
ms.openlocfilehash: 8fcd76ee85c5108aa6209952085d0488b1883256
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506193"
---
# <a name="allow-users-to-send-email-as-a-distribution-group"></a><span data-ttu-id="242ac-102">อนุญาตให้ผู้ใช้ส่งอีเมลที่เป็นกลุ่มการกระจายสินค้า</span><span class="sxs-lookup"><span data-stu-id="242ac-102">Allow users to send email as a distribution group</span></span>

<span data-ttu-id="242ac-103">เมื่อต้องการอนุญาตให้ผู้ใช้ส่งข้อความที่ปรากฏขึ้นมาจากกลุ่มการแจกจ่ายที่มีอยู่ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="242ac-103">To allow users to send messages that appear to come from an existing distribution group, follow these steps:</span></span>

1. <span data-ttu-id="242ac-104">ในการ[แลกเปลี่ยน admin ศูนย์](https://outlook.office365.com/ecp/)ไปที่**ผู้รับ** \> **กลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="242ac-104">In the [Exchange admin center](https://outlook.office365.com/ecp/), go to **Recipients** \> **Groups**.</span></span>

2. <span data-ttu-id="242ac-105">เลือกกลุ่มการกระจายสินค้าที่คุณต้องการแก้ไข และจากนั้น คลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="242ac-105">Select the distribution group you want to modify, and then click **Edit**.</span></span>

3. <span data-ttu-id="242ac-106">ในคุณสมบัติของกลุ่ม ไปที่**การมอบหมายกลุ่ม**แท็บเพื่อระบุผู้ใช้ที่สามารถส่งเป็น หรือในนามของกลุ่มการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="242ac-106">In the properties of the group, go to the **Group delegation** tab to specify the users who can send as or send on behalf of the distribution group.</span></span>

<span data-ttu-id="242ac-107">สำหรับข้อมูลเพิ่มเติม ให้ดู[ตัวเลือกอีเมล](https://technet.microsoft.com/library/bb124513.aspx#groupdelegation)</span><span class="sxs-lookup"><span data-stu-id="242ac-107">For more information, see [Email options](https://technet.microsoft.com/library/bb124513.aspx#groupdelegation).</span></span>
