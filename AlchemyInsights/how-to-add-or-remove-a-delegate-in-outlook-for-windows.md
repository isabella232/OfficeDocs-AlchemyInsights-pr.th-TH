---
title: วิธีการเพิ่มหรือเอาผู้รับมอบสิทธิ์ใน Outlook สำหรับ Windows ออก
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573810"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="64ed5-102">วิธีการเพิ่มหรือเอาผู้รับมอบสิทธิ์ใน Outlook สำหรับ Windows ออก</span><span class="sxs-lookup"><span data-stu-id="64ed5-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="64ed5-103">เมื่อต้องการเพิ่มผู้รับมอบสิทธิ์ใน Outlook สำหรับ Windows:</span><span class="sxs-lookup"><span data-stu-id="64ed5-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="64ed5-104">คลิกที่แท็บ **ไฟล์** ตามด้วย **การตั้งค่าบัญชีผู้** ใช้แล้วเลือกผู้รับ **มอบสิทธิ์การเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="64ed5-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="64ed5-105">คลิก **เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="64ed5-105">Click on **Add**.</span></span> <span data-ttu-id="64ed5-106">ถ้า **เพิ่ม** ไม่ปรากฏแสดงว่าการเชื่อมต่อที่ใช้งานอยู่อาจไม่มีอยู่ระหว่าง Outlook และ Exchange</span><span class="sxs-lookup"><span data-stu-id="64ed5-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="64ed5-107">แถบสถานะของ Outlook จะแสดงสถานะการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="64ed5-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="64ed5-108">พิมพ์ชื่อของบุคคลที่คุณต้องการกำหนดให้เป็นผู้รับมอบสิทธิ์ของคุณหรือค้นหาและเลือกชื่อในรายการผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="64ed5-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="64ed5-109">ผู้รับมอบสิทธิ์ต้องเป็นบุคคลในสมุดรายชื่อส่วนกลางของ Exchange ขององค์กรของคุณ (GAL)</span><span class="sxs-lookup"><span data-stu-id="64ed5-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="64ed5-110">คลิก **เพิ่ม** ตามด้วย **ตกลง**</span><span class="sxs-lookup"><span data-stu-id="64ed5-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="64ed5-111">ในกล่องโต้ตอบสิทธิ์ของผู้รับ **มอบ** สิทธิ์ให้ยอมรับการตั้งค่าสิทธิ์เริ่มต้นหรือเลือกระดับการเข้าถึงแบบกำหนดเองสำหรับโฟลเดอร์ Exchange</span><span class="sxs-lookup"><span data-stu-id="64ed5-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="64ed5-112">ถ้าผู้รับมอบสิทธิ์จำเป็นต้องมีสิทธิ์ในการทำงานกับการเรียกประชุมและการตอบกลับการตั้งค่าสิทธิ์เริ่มต้นเช่นผู้ **รับมอบสิทธิ์จะได้รับสำเนาของข้อความที่เกี่ยวข้องกับการประชุมที่ส่งถึงฉัน** เพียงพอ</span><span class="sxs-lookup"><span data-stu-id="64ed5-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="64ed5-113">คุณสามารถปล่อยให้การตั้งค่าสิทธิ์ใน **กล่องจดหมายเข้า** ที่ **ไม่มี**</span><span class="sxs-lookup"><span data-stu-id="64ed5-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="64ed5-114">การเรียกประชุมและการตอบกลับจะถูกส่งไปยังกล่องจดหมายเข้าของผู้รับมอบสิทธิ์โดยตรง</span><span class="sxs-lookup"><span data-stu-id="64ed5-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="64ed5-115">ตามค่าเริ่มต้นแล้วผู้รับมอบสิทธิ์จะได้รับสิทธิ์ผู้ **แก้ไข (สามารถอ่านสร้างและปรับเปลี่ยนรายการ)** ไปยังโฟลเดอร์ **ปฏิทิน** ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="64ed5-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="64ed5-116">เมื่อผู้รับมอบสิทธิ์ตอบสนองต่อการประชุมในนามของคุณการประชุมจะถูกเพิ่มลงในโฟลเดอร์ **ปฏิทิน** ของคุณโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="64ed5-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="64ed5-117">เมื่อต้องการส่งข้อความเพื่อแจ้งให้ผู้รับมอบสิทธิ์ของสิทธิ์ที่เปลี่ยนแปลงให้เลือกกล่องกาเครื่องหมาย **ส่งข้อความโดยอัตโนมัติไปยังผู้รับมอบสิทธิ์ในการสรุปสิทธิ์เหล่านี้**</span><span class="sxs-lookup"><span data-stu-id="64ed5-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="64ed5-118">ถ้าคุณต้องการให้เลือกกล่องกาเครื่องหมายผู้รับ **มอบสิทธิ์สามารถดูรายการส่วนตัวของฉัน**</span><span class="sxs-lookup"><span data-stu-id="64ed5-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="64ed5-119">การตั้งค่านี้จะมีผลต่อโฟลเดอร์ Exchange ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="64ed5-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="64ed5-120">ซึ่งรวมถึงจดหมายที่ติดต่อปฏิทินงานบันทึกย่อและโฟลเดอร์สมุดบันทึกทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="64ed5-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="64ed5-121">ไม่มีวิธีใดที่จะให้สิทธิ์การเข้าถึงรายการส่วนตัวในโฟลเดอร์ที่ระบุเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="64ed5-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="64ed5-122">เลือก **ตกลง**</span><span class="sxs-lookup"><span data-stu-id="64ed5-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="64ed5-123">ข้อความที่ส่งพร้อมสิทธิ์ส่งในนามรวมทั้งชื่อผู้รับมอบสิทธิ์และชื่อของคุณที่อยู่ถัด **จาก**</span><span class="sxs-lookup"><span data-stu-id="64ed5-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="64ed5-124">เมื่อข้อความถูกส่งด้วยสิทธิ์ส่งเป็นเฉพาะชื่อของคุณเท่านั้นที่จะปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="64ed5-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="64ed5-125">เมื่อคุณเพิ่มบุคคลในฐานะผู้รับมอบสิทธิ์แล้วพวกเขาสามารถเพิ่มกล่องจดหมาย Exchange ของคุณไปยังโปรไฟล์ Outlook ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="64ed5-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="64ed5-126">สำหรับคำแนะนำให้ดู[ที่จัดการจดหมายและรายการปฏิทินของบุคคลอื่น](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)</span><span class="sxs-lookup"><span data-stu-id="64ed5-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="64ed5-127">เมื่อต้องการเอาผู้รับมอบสิทธิ์ใน Outlook สำหรับ Windows:</span><span class="sxs-lookup"><span data-stu-id="64ed5-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="64ed5-128">คลิกแท็บ **ไฟล์**</span><span class="sxs-lookup"><span data-stu-id="64ed5-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="64ed5-129">คลิก **การตั้งค่าบัญชีผู้ใช้** ตามด้วยการเข้าถึงของผู้รับ **มอบสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="64ed5-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="64ed5-130">เลือกชื่อของผู้รับมอบสิทธิ์ที่คุณต้องการเปลี่ยนแปลงสิทธิ์จากนั้นคลิก **เอาออก** ตามด้วย **ตกลง**</span><span class="sxs-lookup"><span data-stu-id="64ed5-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
