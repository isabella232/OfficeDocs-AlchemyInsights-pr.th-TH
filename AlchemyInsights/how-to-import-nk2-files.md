---
title: วิธีการนําเข้า NK2- ไฟล์
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759351"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="c5447-102">วิธีการนําเข้าแฟ้ม.nk2</span><span class="sxs-lookup"><span data-stu-id="c5447-102">How to import .nk2 files</span></span> 

<span data-ttu-id="c5447-103">เมื่อคุณเริ่มใช้งาน Microsoft Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สําหรับ Microsoft 365 เป็นครั้งแรก แคชชื่อเล่นของคุณ (เก็บไว้ในแฟ้ม .nk2*ชื่อ)* จะถูกนําเข้าไปยังข้อความที่ซ่อนไว้ในที่เก็บข้อความเริ่มต้นของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5447-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="c5447-104">เมื่อต้องการนําเข้าแฟ้ม .nk2 ลงใน Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สําหรับ Microsoft 365 โปรดตรวจสอบให้แน่ใจว่า แฟ้ม .nk2 อยู่ในโฟลเดอร์ต่อไปนี้: %appdata%\Microsoft\Outlook Outlook</span><span class="sxs-lookup"><span data-stu-id="c5447-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="c5447-105">**หมายเหตุ**: แฟ้ม.nk2 ต้องมีชื่อเดียวกันกับโปรไฟล์ Outlook 2013 หรือ Outlook 2016 ปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5447-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="c5447-106">โดยค่าเริ่มต้น ชื่อส่วนกําหนดค่าคือ "Outlook"</span><span class="sxs-lookup"><span data-stu-id="c5447-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="c5447-107">เมื่อต้องการตรวจสอบชื่อส่วนกําหนดค่า ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="c5447-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="c5447-108">คลิก**เริ่ม**แล้วคลิก**แผงควบคุม**</span><span class="sxs-lookup"><span data-stu-id="c5447-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="c5447-109">คลิกสองครั้งที่**จดหมาย**</span><span class="sxs-lookup"><span data-stu-id="c5447-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="c5447-110">ในกล่องโต้ตอบ การตั้งค่าจดหมาย ให้เลือก**แสดงโปรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="c5447-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="c5447-111">เลือก**เริ่ม** > **เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="c5447-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="c5447-112">ในกล่อง**เปิด**ให้พิมพ์*outlook.exe /importnk2*แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="c5447-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="c5447-113">หลังจากที่คุณนําเข้าแฟ้ม.nk2 เนื้อหาของแฟ้มจะถูกผสานลงในแคชชื่อเล่นที่มีอยู่ในกล่องจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5447-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="c5447-114">**หมายเหตุ**: แฟ้ม.nk2 ถูกเปลี่ยนชื่อด้วยนามสกุลแฟ้ม.เก่าในครั้งถัดไปที่คุณเริ่ม Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สําหรับ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c5447-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="c5447-115">ถ้าคุณต้องการนําเข้าแฟ้ม.nk2 อีกครั้ง ให้เอานามสกุลของชื่อแฟ้ม .old ออกก่อน</span><span class="sxs-lookup"><span data-stu-id="c5447-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="c5447-116">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การนําเข้าหรือคัดลอกรายการการทําให้สมบูรณ์อัตโนมัติไปยังคอมพิวเตอร์อีกเครื่องหนึ่ง](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)</span><span class="sxs-lookup"><span data-stu-id="c5447-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>