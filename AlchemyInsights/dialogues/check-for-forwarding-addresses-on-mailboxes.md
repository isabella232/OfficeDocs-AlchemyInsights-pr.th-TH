---
title: ตรวจสอบที่อยู่การส่งต่อบนกล่องจดหมาย
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428162"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="393c3-102">ตรวจสอบที่อยู่การส่งต่อบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="393c3-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="393c3-103">บางครั้งแฮกเกอร์ส่งต่อข้อความอีเมลของผู้ใช้ไปยังตัวเอง ดังนั้นก่อนอื่น เราจะตรวจสอบการส่งต่อที่อยู่และกฎบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="393c3-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="393c3-104">จากนั้นเราจะตรวจสอบบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="393c3-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="393c3-105">ต่อไปนี้เป็นวิธีตรวจสอบที่อยู่การส่งต่อ:</span><span class="sxs-lookup"><span data-stu-id="393c3-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="393c3-106">เลือก  >  **ผู้ใช้ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="393c3-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="393c3-107">เลือกผู้ใช้ที่มีบัญชีถูกละเมิด</span><span class="sxs-lookup"><span data-stu-id="393c3-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="393c3-108">ในฟลายเอาท์ที่ปรากฏขึ้น **ให้ขยาย** การตั้งค่าจดหมาย แล้วคลิก **แก้ไข\*\*\*\*เพื่อส่งต่อ** อีเมล</span><span class="sxs-lookup"><span data-stu-id="393c3-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="393c3-109">ลบที่อยู่การส่งต่อที่คุณไม่รู้จักออก</span><span class="sxs-lookup"><span data-stu-id="393c3-109">Remove any forwarding addresses you don't recognize.</span></span>