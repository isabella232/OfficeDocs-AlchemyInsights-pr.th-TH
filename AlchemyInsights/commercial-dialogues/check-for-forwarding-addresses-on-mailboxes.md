---
title: ตรวจสอบที่อยู่การส่งต่อบนกล่องจดหมาย
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403330"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="1131e-102">ตรวจสอบที่อยู่การส่งต่อบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="1131e-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="1131e-103">บางครั้งแฮกเกอร์ส่งต่อข้อความอีเมลของผู้ใช้ไปยังตัวเอง ดังนั้นก่อนอื่น เราจะตรวจสอบการส่งต่อที่อยู่และกฎบนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="1131e-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="1131e-104">จากนั้นเราจะตรวจสอบบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="1131e-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="1131e-105">ต่อไปนี้เป็นวิธีตรวจสอบที่อยู่การส่งต่อ:</span><span class="sxs-lookup"><span data-stu-id="1131e-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="1131e-106">เลือก  >  **ผู้ใช้ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="1131e-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="1131e-107">เลือกผู้ใช้ที่มีบัญชีถูกละเมิด</span><span class="sxs-lookup"><span data-stu-id="1131e-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="1131e-108">ในเมนูปลิวที่ปรากฏขึ้น **ให้ขยาย** การตั้งค่าจดหมาย แล้วคลิก **แก้ไข\*\*\*\*เพื่อส่งต่อ** อีเมล</span><span class="sxs-lookup"><span data-stu-id="1131e-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="1131e-109">ลบที่อยู่การส่งต่อที่คุณไม่รู้จักออก</span><span class="sxs-lookup"><span data-stu-id="1131e-109">Remove any forwarding addresses you don't recognize.</span></span>