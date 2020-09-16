---
title: ลงชื่อเข้าใช้ Windows 10 โดยไม่ใช้รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719972"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="a8eb6-102">ลงชื่อเข้าใช้ Windows 10 โดยไม่ใช้รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="a8eb6-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="a8eb6-103">เมื่อต้องการหลีกเลี่ยงการพิมพ์รหัสผ่านที่ Windows เริ่มต้นเราขอแนะนำให้คุณใช้ตัวเลือกการลงชื่อเข้าใช้ Windows Hello ที่ปลอดภัยเช่น PIN การจดจำใบหน้าหรือลายนิ้วมือถ้าพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="a8eb6-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="a8eb6-104">ถ้าคุณต้องการปิดใช้งานการลงชื่อเข้าใช้ที่ปลอดภัยให้ดูที่คำแนะนำ "ลงชื่อเข้าใช้ Windows 10" โดยอัตโนมัติที่ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="a8eb6-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="a8eb6-105">**การรักษาความปลอดภัยของ Windows Hello ทางเลือกให้กับรหัสผ่านบัญชีผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="a8eb6-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="a8eb6-106">ไปที่ **การตั้งค่า > บัญชีผู้ใช้ > ตัวเลือกการลงชื่อเข้าใช้** (หรือคลิก [ที่นี่](ms-settings:signinoptions?activationSource=GetHelp))</span><span class="sxs-lookup"><span data-stu-id="a8eb6-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a8eb6-107">ตัวเลือกการลงชื่อเข้าใช้ที่พร้อมใช้งานจะแสดงอยู่ในรายการ</span><span class="sxs-lookup"><span data-stu-id="a8eb6-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="a8eb6-108">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="a8eb6-108">For example:</span></span>

![ตัวเลือกการลงชื่อเข้าใช้](media/sign-in-options.png)

<span data-ttu-id="a8eb6-110">คลิกหรือแตะตัวเลือกใดตัวเลือกหนึ่งเพื่อกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="a8eb6-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="a8eb6-111">ครั้งถัดไปที่คุณเริ่มหรือปลดล็อก Windows คุณจะสามารถใช้ตัวเลือกใหม่แทนรหัสผ่านได้</span><span class="sxs-lookup"><span data-stu-id="a8eb6-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="a8eb6-112">**ลงชื่อเข้าใช้ Windows 10 โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="a8eb6-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="a8eb6-113">**หมายเหตุ**: การลงชื่อเข้าใช้โดยอัตโนมัติจะสะดวกแต่จะแนะนำความเสี่ยงด้านความปลอดภัยโดยเฉพาะอย่างยิ่งถ้าพีซีของคุณสามารถเข้าถึงได้โดยผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="a8eb6-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="a8eb6-114">คลิกหรือแตะปุ่ม **เริ่มต้น** ในแถบงาน</span><span class="sxs-lookup"><span data-stu-id="a8eb6-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="a8eb6-115">พิมพ์ **netplwiz** แล้วกดแป้น Enter เพื่อเปิดหน้าต่างบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a8eb6-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="a8eb6-116">ใน **บัญชีผู้ใช้**ให้คลิกบัญชีผู้ใช้ที่คุณต้องการลงชื่อเข้าใช้โดยอัตโนมัติเมื่อ Windows เริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="a8eb6-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="a8eb6-117">ยกเลิกการเลือกกล่องกาเครื่องหมาย "ผู้ใช้ต้องใส่ชื่อผู้ใช้และรหัสผ่านเพื่อใช้คอมพิวเตอร์เครื่องนี้"</span><span class="sxs-lookup"><span data-stu-id="a8eb6-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![ผู้ใช้ต้องใส่ตัวเลือกชื่อผู้ใช้และรหัสผ่าน](media/users-must-enter-username.png)

5. <span data-ttu-id="a8eb6-119">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="a8eb6-119">Click **OK**.</span></span> <span data-ttu-id="a8eb6-120">คุณจะถูกขอให้ใส่และยืนยันรหัสผ่านสำหรับบัญชีผู้ใช้ที่คุณเลือก</span><span class="sxs-lookup"><span data-stu-id="a8eb6-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="a8eb6-121">คลิก **ตกลง** เพื่อเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="a8eb6-121">Click **OK** to finish.</span></span> <span data-ttu-id="a8eb6-122">ครั้งถัดไปที่ Windows 10 จะเริ่มการลงชื่อเข้าใช้บัญชีผู้ใช้ที่คุณเลือกไว้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="a8eb6-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
