---
title: วิธีการนำเข้า-nk2-ไฟล์
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780078"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="341a4-102">วิธีการนำเข้าไฟล์ nk2</span><span class="sxs-lookup"><span data-stu-id="341a4-102">How to import .nk2 files</span></span> 

<span data-ttu-id="341a4-103">เมื่อคุณเริ่ม Microsoft Outlook ๒๐๑๓, Outlook ๒๐๑๖, Outlook ๒๐๑๙หรือ Outlook for Microsoft ๓๖๕เป็นครั้งแรกแคชชื่อเล่นของคุณ (ที่เก็บไว้ในไฟล์ *profilename*) จะถูกนำเข้าไปยังข้อความที่ซ่อนอยู่ในที่เก็บข้อความเริ่มต้นของคุณ</span><span class="sxs-lookup"><span data-stu-id="341a4-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="341a4-104">เมื่อต้องการนำเข้าไฟล์ nk2 ไปยัง Outlook ๒๐๑๓, Outlook ๒๐๑๖, Outlook ๒๐๑๙หรือ Outlook for Microsoft ๓๖๕ตรวจสอบให้แน่ใจว่าไฟล์ nk2 อยู่ในโฟลเดอร์ต่อไปนี้:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="341a4-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="341a4-105">**หมายเหตุ**: ไฟล์ nk2 ต้องมีชื่อเดียวกันกับโปรไฟล์ outlook ๒๐๑๓หรือ outlook ๒๐๑๖ปัจจุบันของคุณ</span><span class="sxs-lookup"><span data-stu-id="341a4-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="341a4-106">ตามค่าเริ่มต้นชื่อโปรไฟล์คือ "Outlook"</span><span class="sxs-lookup"><span data-stu-id="341a4-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="341a4-107">เมื่อต้องการตรวจสอบชื่อโปรไฟล์ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="341a4-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="341a4-108">คลิก**เริ่ม**แล้วคลิก**แผงควบคุม**</span><span class="sxs-lookup"><span data-stu-id="341a4-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="341a4-109">คลิกสองครั้งที่**จดหมาย**</span><span class="sxs-lookup"><span data-stu-id="341a4-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="341a4-110">ในกล่องโต้ตอบการตั้งค่าจดหมายให้เลือก**แสดงโปรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="341a4-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="341a4-111">เลือก**เริ่มต้น**  >  **เรียกใช้**</span><span class="sxs-lookup"><span data-stu-id="341a4-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="341a4-112">ในกล่อง**เปิด**ให้พิมพ์*outlook.exe/Importnk2*แล้วเลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="341a4-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="341a4-113">หลังจากที่คุณนำเข้าไฟล์ nk2 เนื้อหาของไฟล์จะถูกผสานเข้าไปในแคชชื่อเล่นที่มีอยู่แล้วในกล่องจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="341a4-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="341a4-114">**หมายเหตุ**: ไฟล์ nk2 ถูกเปลี่ยนชื่อด้วยนามสกุลของชื่อไฟล์ .old ในครั้งถัดไปที่คุณเริ่ม outlook ๒๐๑๓, outlook ๒๐๑๖, outlook ๒๐๑๙หรือ Outlook for Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="341a4-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="341a4-115">ถ้าต้องการนำเข้าไฟล์ nk2 อีกครั้งให้เอานามสกุลของชื่อไฟล์ .old ออกก่อน</span><span class="sxs-lookup"><span data-stu-id="341a4-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="341a4-116">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่นำเข้าหรือคัดลอกรายการการทำให้สมบูรณ์อัตโนมัติไปยังคอมพิวเตอร์เครื่องอื่น](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)</span><span class="sxs-lookup"><span data-stu-id="341a4-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>