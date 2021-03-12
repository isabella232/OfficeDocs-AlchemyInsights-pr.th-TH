---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749291"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="53677-102">ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="53677-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="53677-103">ต่อไปนี้เป็นวิธีการตั้งค่านโยบายเพื่อย้ายอีเมลเก่าของผู้ใช้ไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ:</span><span class="sxs-lookup"><span data-stu-id="53677-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="53677-104">Go to [**security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data  >  **governance**  >  **Archive** to verify an archive mailbox has been enabled for the user.</span><span class="sxs-lookup"><span data-stu-id="53677-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="53677-105">ถ้ายังไม่ได้เปิด ให้คลิก **เปิดใช้งาน** แล้วคลิก **ใช่** ในกล่องคําเตือน</span><span class="sxs-lookup"><span data-stu-id="53677-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="53677-106">ไปที่ศูนย์ [**การจัดการ Exchange >การจัดการการปฏิบัติตาม>แท็กการเก็บข้อมูล**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="53677-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="53677-107">เลือกไอคอน + แล้วเลือก **ใช้กับกล่องจดหมายทั้งหมด** โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="53677-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="53677-108">กําหนดชื่อให้กับแท็กการเก็บข้อมูล แล้วเลือก **ย้ายไปยังเก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="53677-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="53677-109">ในช่วงเวลาการเก็บข้อมูล ให้ใส่เวลาที่คุณต้องการ เช่น 90 วัน</span><span class="sxs-lookup"><span data-stu-id="53677-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="53677-110">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="53677-110">Click **Save**.</span></span>
5. <span data-ttu-id="53677-111">ตอนนี้ให้สร้างนโยบายการเก็บข้อมูล **โดยเลือก** นโยบายการเก็บข้อมูล เลือกไอคอนเพื่อเพิ่มนโยบายใหม่</span><span class="sxs-lookup"><span data-stu-id="53677-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="53677-112">กําหนดชื่อให้กับนโยบายการเก็บข้อมูล แล้วคลิกและเลื่อนเพื่อค้นหาและเพิ่มแท็กการเก็บข้อมูลที่คุณเพิ่งสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="53677-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="53677-113">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="53677-113">Click **Save**.</span></span>
7. <span data-ttu-id="53677-114">สุดท้าย ให้ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมายของผู้ใช้: ยังคงอยู่ในศูนย์การจัดการ Exchange ให้ไปที่  >  **กล่องจดหมาย** ผู้รับ</span><span class="sxs-lookup"><span data-stu-id="53677-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="53677-115">เลือกผู้ใช้ทั้งหมดที่คุณต้องการปรับใช้นโยบาย แล้วเลือก **แก้ไข** (ไอคอนรูปดินสอ)</span><span class="sxs-lookup"><span data-stu-id="53677-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="53677-116">ในกล่องโต้ตอบ ให้คลิกฟีเจอร์ **ของ** กล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="53677-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="53677-117">ภายใต้ **นโยบายการเก็บ** ข้อมูล ให้ใช้นโยบายที่คุณเพิ่ง>**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="53677-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="53677-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="53677-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
