---
title: เปิดไฟล์แบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745626"
---
# <a name="file-open-read-only"></a><span data-ttu-id="01110-102">เปิดไฟล์แบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="01110-102">File open read-only</span></span>

<span data-ttu-id="01110-103">คุณอาจพบว่าเมื่อคุณกำลังเปิดไฟล์พวกเขาเปิดเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="01110-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="01110-104">ในบางกรณีการทำเช่นนี้มีไว้สำหรับการรักษาความปลอดภัยที่เพิ่มขึ้นเช่นเมื่อคุณกำลังเปิดไฟล์จากอินเทอร์เน็ตและเวลาอื่นๆอาจเป็นเพราะการตั้งค่าที่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="01110-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="01110-105">ต่อไปนี้คือบางสถานการณ์ที่ไฟล์เปิดแบบอ่านอย่างเดียวและขั้นตอนบางอย่างที่คุณสามารถทำได้เพื่อเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="01110-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="01110-106">**โปรแกรมป้องกันไวรัสของฉันก่อให้เกิดการเปิดแบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="01110-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="01110-107">โปรแกรมป้องกันไวรัสบางโปรแกรมอาจปกป้องคุณจากไฟล์ที่อาจไม่ปลอดภัยโดยการเปิดแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="01110-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="01110-108">คุณอาจจำเป็นต้องตรวจสอบกับผู้ให้บริการป้องกันไวรัสของคุณเพื่อเรียนรู้วิธีการปรับการตั้งค่าเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="01110-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="01110-109">BitDefender ตัวอย่างเช่นมีเนื้อหาเกี่ยวกับการเพิ่มข้อยกเว้นของแอปพลิเคชันที่นี่:[วิธีการเพิ่มแอปพลิเคชันหรือการยกเว้นกระบวนการในศูนย์ควบคุม BitDefender](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="01110-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="01110-110">**คุณสมบัติไฟล์ถูกตั้งค่าเป็นแบบอ่านอย่างเดียวหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="01110-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="01110-111">คุณสามารถตรวจสอบคุณสมบัติไฟล์ได้โดยการคลิกขวาที่ไฟล์แล้วเลือกคุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="01110-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="01110-112">ถ้ามีการเลือกแอตทริบิวต์แบบอ่านอย่างเดียวแล้วคุณสามารถยกเลิกการเลือกได้แล้วคลิกตกลง</span><span class="sxs-lookup"><span data-stu-id="01110-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="01110-113">**เนื้อหาอยู่ในมุมมองที่ได้รับการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="01110-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="01110-114">ไฟล์จากอินเทอร์เน็ตและจากตำแหน่งที่ตั้งอื่นที่อาจไม่ปลอดภัยอาจมีไวรัสเวิร์มหรือมัลแวร์ชนิดอื่นๆที่อาจเป็นอันตรายต่อคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="01110-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="01110-115">นอกจากนี้ยังเป็นกรณีที่มีสิ่งที่แนบมากับอีเมลหรือไฟล์ที่คุณดาวน์โหลดแล้ว</span><span class="sxs-lookup"><span data-stu-id="01110-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="01110-116">เมื่อต้องการช่วยปกป้องคอมพิวเตอร์ของคุณไฟล์จากตำแหน่งที่ตั้งที่อาจไม่ปลอดภัยเหล่านี้จะถูกเปิดในมุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="01110-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="01110-117">โดยการใช้มุมมองที่ได้รับการป้องกันคุณสามารถอ่านไฟล์และดูเนื้อหาได้ในขณะที่ลดความเสี่ยง</span><span class="sxs-lookup"><span data-stu-id="01110-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="01110-118">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับมุมมองที่ได้รับการป้องกันและวิธีการเปลี่ยนแปลงการตั้งค่าให้ดูบทความนี้: [มุมมองที่ได้รับการป้องกันคืออะไร](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="01110-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="01110-119">**OneDrive เต็มแล้วหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="01110-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="01110-120">ถ้าไฟล์ถูกจัดเก็บไว้ใน OneDrive และพื้นที่เก็บข้อมูล OneDrive ของคุณเต็มคุณจะไม่สามารถบันทึกเอกสารได้จนกว่าคุณจะอยู่ภายใต้พื้นที่ที่กำหนดของคุณ</span><span class="sxs-lookup"><span data-stu-id="01110-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="01110-121">คุณสามารถตรวจสอบพื้นที่ว่างของคุณบน OneDrive ได้โดยการคลิกไอคอน OneDrive ในศูนย์การแจ้งเตือนและเลือกจัดการที่เก็บข้อมูลหรือคุณสามารถไปที่ [https://onedrive.live.com](https://onedrive.live.com) ลงชื่อเข้าใช้และบันทึกจำนวนพื้นที่ที่ใช้ที่ด้านล่างซ้ายของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="01110-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="01110-122">**เปิดใช้งาน Office แล้วใช่หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="01110-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="01110-123">ถ้า Office ไม่ได้เปิดใช้งานหรือถ้าการสมัครใช้งานของคุณหมดอายุแล้วคุณอาจอยู่ในโหมดการลดฟังก์ชันการทำงานแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="01110-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="01110-124">สำหรับข้อมูลเกี่ยวกับวิธีการเปิดใช้งาน Office ให้ดู [ที่ข้อผิดพลาดผลิตภัณฑ์ที่](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)ไม่มีสิทธิ์การใช้งานและการเปิดใช้งานใน Office</span><span class="sxs-lookup"><span data-stu-id="01110-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="01110-125">**ถ้าทั้งหมดอื่นล้มเหลว ...**</span><span class="sxs-lookup"><span data-stu-id="01110-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="01110-126">ลองเริ่มต้นระบบคอมพิวเตอร์ใหม่</span><span class="sxs-lookup"><span data-stu-id="01110-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="01110-127">ติดตั้งการอัปเดต Office</span><span class="sxs-lookup"><span data-stu-id="01110-127">Install Office updates</span></span>
    
- <span data-ttu-id="01110-128">ดำเนินการซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="01110-128">Perform an Online repair of Office</span></span>
    

