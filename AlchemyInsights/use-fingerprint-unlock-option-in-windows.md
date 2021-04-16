---
title: ใช้ตัวเลือกการปลดล็อกลายนิ้วมือใน Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796696"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2aa1d-102">ใช้ตัวเลือกการปลดล็อกลายนิ้วมือใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="2aa1d-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2aa1d-103">**เปิดใช้งานการตรวจสอบลายนิ้วมือของ Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="2aa1d-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2aa1d-104">เมื่อต้องการปลดล็อก Windows 10 โดยใช้ลายนิ้วมือของคุณ คุณจะต้องตั้งค่าลายนิ้วมือของ Windows Hello โดยการเพิ่ม (เพื่อให้ Windows เรียนรู้การรู้รู้) อย่างน้อยหนึ่งนิ้ว</span><span class="sxs-lookup"><span data-stu-id="2aa1d-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2aa1d-105">ไปที่ **การตั้งค่า >บัญชีผู้ใช้> ตัวเลือกการ** ลงชื่อเข้าใช้ (หรือ [คลิกที่นี่](ms-settings:signinoptions?activationSource=GetHelp))</span><span class="sxs-lookup"><span data-stu-id="2aa1d-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2aa1d-106">ตัวเลือกการลงชื่อเข้าใช้ที่พร้อมใช้งานจะแสดงในรายการ</span><span class="sxs-lookup"><span data-stu-id="2aa1d-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2aa1d-107">ตัวอย่างเช่น:</span><span class="sxs-lookup"><span data-stu-id="2aa1d-107">For example:</span></span>

    ![ตัวเลือกการลงชื่อเข้าใช้](media/sign-in-options.png)

2. <span data-ttu-id="2aa1d-109">คลิกหรือ **แตะ ลายนิ้วมือ** Windows Hello **แล้วคลิก** ตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="2aa1d-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2aa1d-110">ในหน้าต่างการตั้งค่า Windows Hello **ให้คลิก** เริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2aa1d-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2aa1d-111">เซนเซอร์ลายนิ้วมือจะเปิดใช้งาน และคุณจะถูกขอให้วางนิ้วของคุณบนเซ็นเซอร์:</span><span class="sxs-lookup"><span data-stu-id="2aa1d-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![เซนเซอร์ลายนิ้วมือ](media/fingerprint-sensor.png)

3. <span data-ttu-id="2aa1d-113">ให้ปฏิบัติตามคําแนะนํา ซึ่งจะขอให้คุณสแกนนิ้วซ้ําๆ</span><span class="sxs-lookup"><span data-stu-id="2aa1d-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2aa1d-114">เมื่อเสร็จสิ้น คุณจะมีตัวเลือกในการเพิ่มนิ้วอื่นๆ ที่คุณอาจต้องการใช้ในการลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="2aa1d-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2aa1d-115">ในครั้งถัดไปที่คุณลงชื่อเข้าใช้ Windows 10 คุณจะมีตัวเลือกในการใช้ลายนิ้วมือเพื่อบันทึก</span><span class="sxs-lookup"><span data-stu-id="2aa1d-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2aa1d-116">**ลายนิ้วมือของ Windows Hello ไม่พร้อมใช้งานเป็นตัวเลือกการลงชื่อเข้าใช้**</span><span class="sxs-lookup"><span data-stu-id="2aa1d-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2aa1d-117">ถ้าลายนิ้วมือของ Windows Hello ไม่ได้แสดงเป็นตัวเลือกในตัวเลือกการลงชื่อเข้าใช้ นั่นหมายความว่า Windows ไม่ทราบถึงตัวอ่าน/สแกนเนอร์ลายนิ้วมือที่ต่ออยู่กับพีซีของคุณ หรือนโยบายระบบป้องกันไม่ให้มีการใช้งาน (ตัวอย่างเช่น ถ้าพีซีของคุณถูกจัดการโดยที่ทํางานของคุณ)</span><span class="sxs-lookup"><span data-stu-id="2aa1d-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2aa1d-118">เมื่อต้องการแก้ไขปัญหา:</span><span class="sxs-lookup"><span data-stu-id="2aa1d-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2aa1d-119">เลือก **ปุ่ม** เริ่ม ในแถบงาน แล้วค้นหา **ตัวจัดการ** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2aa1d-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2aa1d-120">คลิกหรือแตะเพื่อเปิด **ตัวจัดการ** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2aa1d-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2aa1d-121">ใน Device Manager ให้ขยายอุปกรณ์ชีวมาตรโดยคลิกที่เครื่องหมายบั้ง</span><span class="sxs-lookup"><span data-stu-id="2aa1d-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![อุปกรณ์ทางชีวภาพ](media/biometric-devices.png)

4. <span data-ttu-id="2aa1d-123">ตัวสแกนลายนิ้วมือของคุณควรแสดงรายการเป็นอุปกรณ์ชีวมาตร เช่น ตัวสแกน Synaptics WBDI ดังนี้</span><span class="sxs-lookup"><span data-stu-id="2aa1d-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![อุปกรณ์ทางชีวภาพ](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2aa1d-125">ถ้าตัวสแกนลายนิ้วมือของคุณไม่แสดงขึ้น และสแกนเนอร์ถูกรวมเข้ากับพีซีของคุณ ให้ไปที่เว็บไซต์ของผู้ผลิตพีซี</span><span class="sxs-lookup"><span data-stu-id="2aa1d-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2aa1d-126">ในส่วนการสนับสนุนทางเทคนิคของรุ่นพีซีของคุณ ให้ค้นหาโปรแกรมควบคุม Windows 10 เพื่อสแกนที่คุณสามารถติดตั้งได้</span><span class="sxs-lookup"><span data-stu-id="2aa1d-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2aa1d-127">ถ้าสแกนเนอร์แยกจากพีซี (ต่อผ่าน USB) ไปที่เว็บไซต์ของผู้ผลิตสแกนเนอร์เพื่อค้นหาและติดตั้งซอฟต์แวร์โปรแกรมควบคุมอุปกรณ์ Windows 10 ของรุ่นสแกนเนอร์ที่คุณมี</span><span class="sxs-lookup"><span data-stu-id="2aa1d-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
