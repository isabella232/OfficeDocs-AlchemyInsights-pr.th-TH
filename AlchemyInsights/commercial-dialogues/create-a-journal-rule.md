---
title: การสร้างกฎของบันทึกรายวัน
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: b0b95f8b6460418d92314dede2ca8bc1326b033e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747894"
---
# <a name="create-a-journal-rule"></a><span data-ttu-id="e8e4e-102">การสร้างกฎของบันทึกรายวัน</span><span class="sxs-lookup"><span data-stu-id="e8e4e-102">Create a journal rule</span></span>

<span data-ttu-id="e8e4e-103">โดยมีวิธีการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e8e4e-103">Here's how:</span></span>

1. <span data-ttu-id="e8e4e-104">ใน [ศูนย์การจัดการ Exchange](https://go.microsoft.com/fwlink/p/?linkid=2059104)ให้ไปที่กฎ **บันทึกการจัดการ** การปฏิบัติตามนโยบาย  >  แล้วเลือกไอคอนเพิ่ม **(+)**</span><span class="sxs-lookup"><span data-stu-id="e8e4e-104">In the [Exchange admin center](https://go.microsoft.com/fwlink/p/?linkid=2059104), go to **compliance management** > **journal rules**, and then select the **Add (+)** icon.</span></span>
2. <span data-ttu-id="e8e4e-105">ใน **กฎบันทึก** ใหม่ ให้ระบุชื่อกฎบันทึกรายวัน แล้วลงแข่งขันกับเขตข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e8e4e-105">In **new journal rule**, provide a name for the journal rule and then compete the following fields:</span></span>  
    - <span data-ttu-id="e8e4e-106">**ส่งรายงานบันทึกรายวัน** ไปยัง : ใส่ที่อยู่ของกล่องจดหมายบันทึกรายวันที่จะได้รับรายงานบันทึกรายวันทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e8e4e-106">**Send journal reports to**: Enter the address of the journaling mailbox that will receive all the journal reports.</span></span>  
    - <span data-ttu-id="e8e4e-107">**ถ้าข้อความถูกส่งถึงหรือได้รับจาก**: ระบุผู้รับที่จะตั้งกฎเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="e8e4e-107">**If the message is sent to or received from**: Specify the recipient that the rule will target.</span></span> <span data-ttu-id="e8e4e-108">คุณสามารถเลือกผู้รับที่ระบุหรือปรับใช้กฎกับข้อความทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e8e4e-108">You can either select a specific recipient or apply the rule to all messages.</span></span>  
    - <span data-ttu-id="e8e4e-109">**บันทึกรายวันข้อความ** ต่อไปนี้ ระบุขอบเขตของกฎบันทึกรายวัน</span><span class="sxs-lookup"><span data-stu-id="e8e4e-109">**Journal the following messages**: Specify the scope of the journal rule.</span></span> <span data-ttu-id="e8e4e-110">คุณสามารถบันทึกบันทึกภาพได้เฉพาะข้อความภายใน เท่านั้น เฉพาะข้อความภายนอก หรือข้อความทั้งหมดโดยไม่เกี่ยวกับจุดเริ่มต้นหรือปลายทาง</span><span class="sxs-lookup"><span data-stu-id="e8e4e-110">You can journal only the internal messages, only the external messages, or all messages regardless of origin or destination.</span></span>
3. <span data-ttu-id="e8e4e-111">เลือกบันทึก เพื่อสร้างกฎบันทึกรายวัน</span><span class="sxs-lookup"><span data-stu-id="e8e4e-111">Select **Save** to create the journal rule.</span></span>
