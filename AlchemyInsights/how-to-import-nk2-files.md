---
title: how-เพื่อนำเข้า-nk2-แฟ้ม
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: ed0c679cf3ed9d363e552c04a5ae6d0fc72f88dd
ms.sourcegitcommit: 6a229919cf67005e7e67841e9e45f2f3aa6833ef
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630034"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="f4eae-102">วิธีการนำเข้าแฟ้ม.nk2</span><span class="sxs-lookup"><span data-stu-id="f4eae-102">How to import .nk2 files</span></span> 

<span data-ttu-id="f4eae-103">เมื่อคุณเริ่ม Microsoft Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สำหรับ Office 365 เป็นครั้งแรก แคชชื่อเล่นของคุณ (ถูกเก็บในแฟ้ม.nk2 *profilename*) มีการนำเข้าลงในข้อความที่ซ่อนไว้ในที่เก็บข้อความเริ่มต้นของคุณ</span><span class="sxs-lookup"><span data-stu-id="f4eae-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="f4eae-104">การนำเข้าแฟ้ม.nk2 ใน Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สำหรับ Office 365 โปรดตรวจสอบให้แน่ใจว่า แฟ้ม.nk2 อยู่ในโฟลเดอร์ต่อไปนี้: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="f4eae-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="f4eae-105">**หมายเหตุ**: แฟ้ม.nk2 ต้องมีชื่อเดียวกับโปรไฟล์ Outlook 2013 หรือ Outlook 2016 ปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="f4eae-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="f4eae-106">โดยค่าเริ่มต้น ชื่อส่วนกำหนดค่าให้เป็น "Outlook"</span><span class="sxs-lookup"><span data-stu-id="f4eae-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="f4eae-107">เมื่อต้องการตรวจสอบชื่อโปรไฟล์ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f4eae-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="f4eae-108">คลิก**เริ่ม**และจากนั้น คลิก **'แผงควบคุม'**</span><span class="sxs-lookup"><span data-stu-id="f4eae-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="f4eae-109">คลิกสองครั้งที่**จดหมาย**</span><span class="sxs-lookup"><span data-stu-id="f4eae-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="f4eae-110">ในกล่องโต้ตอบการตั้งค่าจดหมาย เลือก**แสดงโปรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="f4eae-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="f4eae-111">เลือก**เริ่ม** > **เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="f4eae-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="f4eae-112">ในกล่อง**เปิด**พิมพ์*outlook.exe /importnk2*และจากนั้น ให้เลือก **'ตกลง'**</span><span class="sxs-lookup"><span data-stu-id="f4eae-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="f4eae-113">หลังจากที่คุณนำเข้าแฟ้ม.nk2 เนื้อหาของแฟ้มจะถูกผสานลงในแคชชื่อเล่นที่มีอยู่ถูกเก็บไว้ในกล่องจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="f4eae-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="f4eae-114">**หมายเหตุ**: แฟ้ม.nk2 ถูกเปลี่ยนชื่อ ด้วยนามสกุลเป็น.old ในครั้งถัดไปที่คุณเริ่ม Outlook 2013, Outlook 2016, Outlook 2019 หรือ Outlook สำหรับ Office 365</span><span class="sxs-lookup"><span data-stu-id="f4eae-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365.</span></span> <span data-ttu-id="f4eae-115">ถ้าต้องการนำเข้าแฟ้ม.nk2 อีกครั้ง เอาออกส่วนขยายชื่อแฟ้ม.old ครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="f4eae-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="f4eae-116">ดูข้อมูลเพิ่มเติม[นำเข้าหรือคัดลอกรายการการทำให้สมบูรณ์อัตโนมัติกับคอมพิวเตอร์เครื่องอื่น](https://support.microsoft.com/en-us/help/2806550/how-to-import-nk2-files-into-outlook%)</span><span class="sxs-lookup"><span data-stu-id="f4eae-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/en-us/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>