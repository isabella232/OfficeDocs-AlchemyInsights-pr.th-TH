---
title: ลงชื่อเข้าใช้ Windows 10 โดยไม่ต้องใช้รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830565"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="d9c67-102">ลงชื่อเข้าใช้ Windows 10 โดยไม่ต้องใช้รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="d9c67-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="d9c67-103">เพื่อหลีกเลี่ยงไม่ให้ต้องพิมพ์รหัสผ่านเมื่อเริ่มต้นระบบ Windows เราขอแนะนนะให้คุณใช้หนึ่งในตัวเลือกการลงชื่อเข้าใช้ที่ปลอดภัยของ Windows Hello เช่น PIN การรู้รู้ใบหน้า หรือลายนิ้วมือ ถ้ามี</span><span class="sxs-lookup"><span data-stu-id="d9c67-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="d9c67-104">ถ้าคุณต้องการปิดใช้งานการลงชื่อเข้าใช้อย่างปลอดภัย ให้ดูคําแนะนํา "ลงชื่อเข้าใช้ Windows 10 โดยอัตโนมัติ" ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="d9c67-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="d9c67-105">**รักษาความปลอดภัยทางเลือกของ Windows Hello ในรหัสผ่านบัญชี**</span><span class="sxs-lookup"><span data-stu-id="d9c67-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="d9c67-106">ไปที่ **การตั้งค่า >บัญชีผู้ใช้> ตัวเลือกการ** ลงชื่อเข้าใช้ (หรือ [คลิกที่นี่](ms-settings:signinoptions?activationSource=GetHelp))</span><span class="sxs-lookup"><span data-stu-id="d9c67-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d9c67-107">ตัวเลือกการลงชื่อเข้าใช้ที่พร้อมใช้งานจะแสดงในรายการ</span><span class="sxs-lookup"><span data-stu-id="d9c67-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="d9c67-108">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="d9c67-108">For example:</span></span>

![ตัวเลือกการลงชื่อเข้าใช้](media/sign-in-options.png)

<span data-ttu-id="d9c67-110">คลิกหรือแตะตัวเลือกใดตัวเลือกหนึ่งเพื่อกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="d9c67-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="d9c67-111">ในครั้งถัดไปที่คุณเริ่มหรือปลดล็อก Windows คุณจะสามารถใช้ตัวเลือกใหม่แทนรหัสผ่านได้</span><span class="sxs-lookup"><span data-stu-id="d9c67-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="d9c67-112">**ลงชื่อเข้าใช้ Windows 10 โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="d9c67-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="d9c67-113">**หมายเหตุ**: การลงชื่อเข้าใช้อัตโนมัติสะดวก แต่มีความเสี่ยงด้านความปลอดภัย โดยเฉพาะถ้าบุคคลหลายคนสามารถเข้าถึงได้จากพีซีของคุณ</span><span class="sxs-lookup"><span data-stu-id="d9c67-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="d9c67-114">คลิกหรือ **แตะ** ปุ่ม เริ่ม ในแถบงาน</span><span class="sxs-lookup"><span data-stu-id="d9c67-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="d9c67-115">พิมพ์ **netplwiz** แล้วกดแป้น Enter เพื่อเปิดหน้าต่างบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d9c67-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="d9c67-116">**ใน บัญชีผู้ใช้** ให้คลิกบัญชีที่คุณต้องการลงชื่อเข้าใช้โดยอัตโนมัติเมื่อ Windows เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="d9c67-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="d9c67-117">ยกเลิกการเลือกกล่องกาเครื่องหมาย "ผู้ใช้ต้องใส่ชื่อผู้ใช้และรหัสผ่านเพื่อใช้คอมพิวเตอร์เครื่องนี้"</span><span class="sxs-lookup"><span data-stu-id="d9c67-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![ผู้ใช้ต้องใส่ตัวเลือกชื่อผู้ใช้และรหัสผ่าน](media/users-must-enter-username.png)

5. <span data-ttu-id="d9c67-119">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="d9c67-119">Click **OK**.</span></span> <span data-ttu-id="d9c67-120">คุณจะถูกขอให้ใส่และยืนยันรหัสผ่านของบัญชีที่คุณเลือก</span><span class="sxs-lookup"><span data-stu-id="d9c67-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="d9c67-121">คลิก **ตกลง** เพื่อเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="d9c67-121">Click **OK** to finish.</span></span> <span data-ttu-id="d9c67-122">เมื่อ Windows 10 เริ่มต้นในครั้งถัดไป Windows 10 จะลงชื่อเข้าใช้บัญชีที่คุณเลือกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="d9c67-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
