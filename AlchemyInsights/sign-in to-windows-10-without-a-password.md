---
title: ลงชื่อเข้าใช้ Windows 10 โดยไม่ต้องใช้รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588299"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="e6da6-102">ลงชื่อเข้าใช้ Windows 10 โดยไม่ต้องใช้รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="e6da6-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="e6da6-103">เมื่อต้องการหลีกเลี่ยงการพิมพ์รหัสผ่านใน Windows startup เราขอแนะนำให้คุณใช้ตัวเลือกการลงชื่อเข้าใช้ Windows Hello ที่ปลอดภัยเช่น PIN การจดจำใบหน้าหรือลายนิ้วมือถ้ามี</span><span class="sxs-lookup"><span data-stu-id="e6da6-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="e6da6-104">ถ้าคุณต้องการปิดใช้งานการลงชื่อเข้าใช้ที่ปลอดภัยให้ดูคำแนะนำ "ลงชื่อเข้าใช้ Windows 10" โดยอัตโนมัติด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="e6da6-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="e6da6-105">**การรักษาความปลอดภัยของ Windows สวัสดีทางเลือกในการรหัสผ่านของบัญชี**</span><span class="sxs-lookup"><span data-stu-id="e6da6-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="e6da6-106">ไปที่**การตั้งค่า > บัญชี > ตัวเลือกการลงชื่อเข้าใช้**(หรือคลิกที่[นี่](ms-settings:signinoptions?activationSource=GetHelp))</span><span class="sxs-lookup"><span data-stu-id="e6da6-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e6da6-107">ตัวเลือกการเข้าสู่ระบบที่พร้อมใช้งานจะแสดงรายการ</span><span class="sxs-lookup"><span data-stu-id="e6da6-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="e6da6-108">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="e6da6-108">For example:</span></span>

![ตัวเลือกการลงชื่อเข้าใช้](media/sign-in-options.png)

<span data-ttu-id="e6da6-110">คลิกหรือแตะหนึ่งในตัวเลือกเพื่อกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="e6da6-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="e6da6-111">ครั้งต่อไปที่คุณเริ่มหรือปลดล็อก Windows คุณจะสามารถใช้ตัวเลือกใหม่แทนรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="e6da6-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="e6da6-112">**ลงชื่อเข้าใช้ Windows 10 โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="e6da6-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="e6da6-113">**หมายเหตุ**: การลงชื่อเข้าใช้โดยอัตโนมัติจะสะดวกแต่จะแนะนำความเสี่ยงด้านความปลอดภัยโดยเฉพาะอย่างยิ่งถ้าพีซีของคุณสามารถเข้าถึงได้โดยผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="e6da6-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="e6da6-114">คลิกหรือเคาะปุ่ม**เริ่มต้น**ในแถบงาน</span><span class="sxs-lookup"><span data-stu-id="e6da6-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="e6da6-115">พิมพ์**netplwiz**และกดแป้น Enter เพื่อเปิดหน้าต่างบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e6da6-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="e6da6-116">ใน**บัญชีผู้ใช้**ให้คลิกบัญชีที่คุณต้องการลงชื่อเข้าใช้โดยอัตโนมัติเมื่อ Windows เริ่มทำงาน</span><span class="sxs-lookup"><span data-stu-id="e6da6-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="e6da6-117">ยกเลิกการเลือกช่องทำเครื่องหมาย "ผู้ใช้ต้องใส่ชื่อผู้ใช้และรหัสผ่านเพื่อใช้คอมพิวเตอร์เครื่องนี้"</span><span class="sxs-lookup"><span data-stu-id="e6da6-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![ผู้ใช้ต้องใส่ตัวเลือกชื่อผู้ใช้และรหัสผ่าน](media/users-must-enter-username.png)

5. <span data-ttu-id="e6da6-119">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="e6da6-119">Click **OK**.</span></span> <span data-ttu-id="e6da6-120">ระบบจะขอให้คุณป้อนและยืนยันรหัสผ่านของบัญชีที่คุณเลือก</span><span class="sxs-lookup"><span data-stu-id="e6da6-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="e6da6-121">คลิ**กตกลง**เมื่อต้องการเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="e6da6-121">Click **OK** to finish.</span></span> <span data-ttu-id="e6da6-122">ครั้งถัดไป Windows 10 เริ่มต้นมันจะลงชื่อเข้าใช้บัญชีที่คุณเลือกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="e6da6-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
