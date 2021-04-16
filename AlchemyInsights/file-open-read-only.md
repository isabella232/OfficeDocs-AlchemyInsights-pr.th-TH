---
title: ไฟล์เปิดแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813203"
---
# <a name="file-open-read-only"></a><span data-ttu-id="ebd25-102">ไฟล์เปิดแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebd25-102">File open read-only</span></span>

<span data-ttu-id="ebd25-103">คุณอาจพบว่าเมื่อคุณเปิดไฟล์ ไฟล์จะเปิดเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebd25-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="ebd25-104">ในบางกรณี ตัวเลือกนี้มีไว้เพื่อเพิ่มความปลอดภัย เช่น เมื่อคุณเปิดไฟล์จากอินเทอร์เน็ต และบางครั้งอาจเกิดจากการตั้งค่าที่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="ebd25-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="ebd25-105">ต่อไปนี้เป็นสถานการณ์ที่ไฟล์เปิดแบบอ่านอย่างเดียวและขั้นตอนบางอย่างที่คุณสามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="ebd25-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="ebd25-106">**โปรแกรมป้องกันไวรัสเป็นสาเหตุให้เปิดแบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="ebd25-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="ebd25-107">โปรแกรมป้องกันไวรัสบางตัวอาจปกป้องคุณจากไฟล์ที่อาจไม่ปลอดภัยโดยการเปิดไฟล์เหล่านั้นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebd25-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="ebd25-108">คุณอาจต้องตรวจสอบกับผู้ให้บริการโปรแกรมป้องกันไวรัสเพื่อเรียนรู้วิธีการปรับการตั้งค่าเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="ebd25-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="ebd25-109">ตัวอย่างเช่น BitDefender มีเนื้อหาเกี่ยวกับการเพิ่มการแยกแอปพลิเคชันออกที่นี่: วิธีการเพิ่มการแยกแอปพลิเคชันหรือกระบวนการในศูนย์ควบคุม[Bitdefender](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="ebd25-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="ebd25-110">**คุณสมบัติไฟล์ถูกตั้งค่าเป็นแบบอ่านอย่างเดียวหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="ebd25-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="ebd25-111">คุณสามารถตรวจสอบคุณสมบัติไฟล์ได้โดยการคลิกขวาที่ไฟล์ แล้วเลือก คุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="ebd25-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="ebd25-112">ถ้าแอตทริบิวต์อ่านอย่างเดียวถูกเลือกไว้ คุณสามารถยกเลิกการเลือกได้แล้วคลิก ตกลง</span><span class="sxs-lookup"><span data-stu-id="ebd25-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="ebd25-113">**เนื้อหาอยู่ในมุมมองที่ได้รับการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="ebd25-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="ebd25-114">ไฟล์จากอินเทอร์เน็ตและจากสถานที่ที่อาจไม่ปลอดภัยอาจมีไวรัส หนอนไวรัส หรือมัลแวร์ชนิดอื่นๆ ที่อาจเป็นอันตรายต่อคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="ebd25-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="ebd25-115">ซึ่งมักเป็นกรณีที่มีสิ่งที่แนบมาในอีเมลหรือไฟล์ที่คุณดาวน์โหลด</span><span class="sxs-lookup"><span data-stu-id="ebd25-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="ebd25-116">เพื่อช่วยปกป้องคอมพิวเตอร์ของคุณ ไฟล์จากที่ตั้งที่อาจไม่ปลอดภัยเหล่านี้จะเปิดขึ้นในมุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="ebd25-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="ebd25-117">เมื่อใช้มุมมองที่ได้รับการป้องกัน คุณสามารถอ่านไฟล์และดูเนื้อหาได้ในขณะที่ลดความเสี่ยง</span><span class="sxs-lookup"><span data-stu-id="ebd25-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="ebd25-118">ดูข้อมูลเพิ่มเติมเกี่ยวกับมุมมองที่ได้รับการป้องกันและวิธีการเปลี่ยนการตั้งค่าได้ ดูบทความนี้: [มุมมองที่ได้รับการป้องกันคืออะไร](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="ebd25-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="ebd25-119">**OneDrive เต็มหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="ebd25-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="ebd25-120">ถ้าไฟล์ถูกเก็บไว้บน OneDrive และพื้นที่เก็บข้อมูล OneDrive ของคุณเต็ม คุณจะไม่สามารถบันทึกเอกสารได้จนกว่าคุณจะอยู่ในพื้นที่ที่จัดสรรแล้ว</span><span class="sxs-lookup"><span data-stu-id="ebd25-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="ebd25-121">คุณสามารถตรวจสอบพื้นที่ว่างของคุณบน OneDrive ได้โดยการคลิกไอคอน OneDrive ในศูนย์การแจ้งเตือนแล้วเลือก จัดการที่เก็บข้อมูล หรือคุณสามารถไปที่ ลงชื่อเข้าใช้ และจดบันทึกจํานวนของพื้นที่ที่ใช้แล้วที่ด้านซ้าย [https://onedrive.live.com](https://onedrive.live.com) ล่างของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="ebd25-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="ebd25-122">**เปิดใช้งาน Office แล้วใช่หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="ebd25-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="ebd25-123">ถ้าไม่ได้เปิดใช้งาน Office หรือถ้าการสมัครใช้งานของคุณหมดอายุ คุณอาจอยู่ในโหมดลดฟังก์ชันการทํางานแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebd25-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="ebd25-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="ebd25-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="ebd25-125">**ถ้าทั้งหมดล้มเหลว...**</span><span class="sxs-lookup"><span data-stu-id="ebd25-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="ebd25-126">ลองรีสตาร์ตคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="ebd25-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="ebd25-127">ติดตั้งการอัปเดต Office</span><span class="sxs-lookup"><span data-stu-id="ebd25-127">Install Office updates</span></span>
    
- <span data-ttu-id="ebd25-128">ซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="ebd25-128">Perform an Online repair of Office</span></span>
    

