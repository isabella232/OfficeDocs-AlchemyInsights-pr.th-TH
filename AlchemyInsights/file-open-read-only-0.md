---
title: เปิดแฟ้มแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: be232b682b7bb3d24f59ad10501edbd796e6bcaf
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401772"
---
# <a name="file-open-read-only"></a><span data-ttu-id="ebad4-102">เปิดแฟ้มแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebad4-102">File open read-only</span></span>

<span data-ttu-id="ebad4-103">คุณอาจพบว่า เมื่อคุณกำลังเปิดแฟ้ม เปิดเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebad4-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="ebad4-104">ในบางกรณี นี่คือความปลอดภัยที่เพิ่ม เช่นเมื่อคุณกำลังเปิดแฟ้มจากอินเทอร์เน็ต และบางครั้ง ดังกล่าวอาจเกิดจากการตั้งค่าที่คุณสามารถเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="ebad4-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="ebad4-105">มีบางสถานการณ์ที่เปิดแฟ้มเป็นแบบอ่านอย่างเดียวและบางขั้นตอนที่คุณสามารถทำการเปลี่ยนแปลงที่นี่</span><span class="sxs-lookup"><span data-stu-id="ebad4-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="ebad4-106">**โปรแกรมป้องกันไวรัสของฉันเป็นสาเหตุให้เปิดแบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="ebad4-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="ebad4-107">โปรแกรมป้องกันไวรัสบางโปรแกรมอาจป้องกันคุณจากแฟ้มที่อาจไม่ปลอดภัย ด้วยการเปิดแฟ้มแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="ebad4-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="ebad4-108">คุณอาจต้องตรวจสอบกับผู้ให้บริการโปรแกรมป้องกันไวรัสเพื่อเรียนรู้วิธีปรับการตั้งค่าเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="ebad4-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="ebad4-109">BitDefender ตัวอย่าง มีเนื้อหาในการเพิ่มการยกเว้นแอพลิเคชันที่นี่:[วิธีการเพิ่มแอพลิเคชันหรือแยกกระบวนการในศูนย์ควบคุม Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl)</span><span class="sxs-lookup"><span data-stu-id="ebad4-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="ebad4-110">**มีคุณสมบัติของแฟ้มตั้งค่าเป็นแบบอ่านอย่างเดียวหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="ebad4-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="ebad4-111">คุณสามารถตรวจสอบคุณสมบัติของแฟ้มได้ ด้วยการคลิกขวาที่แฟ้ม แล้วเลือกคุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="ebad4-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="ebad4-112">ถ้ามีเลือกแอททริบิวต์แบบอ่านอย่างเดียว คุณสามารถยกเลิกเลือกนั้น และคลิกตกลง</span><span class="sxs-lookup"><span data-stu-id="ebad4-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="ebad4-113">**เนื้อหาอยู่ในมุมมองที่ได้รับการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="ebad4-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="ebad4-114">แฟ้ม จากอินเทอร์เน็ต และ จากตำแหน่งที่ตั้งอื่น ๆ อาจไม่ปลอดภัยอาจประกอบด้วยไวรัส เวิร์ม หรือชนิดอื่น ๆ ของมัลแวร์ที่อาจเป็นอันตรายต่อคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="ebad4-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="ebad4-115">นี่คือโดยทั่วไปในกรณีของสิ่งที่แนบทางอีเมลหรือแฟ้มที่คุณดาวน์โหลด</span><span class="sxs-lookup"><span data-stu-id="ebad4-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="ebad4-116">เพื่อช่วยปกป้องคอมพิวเตอร์ของคุณ มีเปิดแฟ้มจากตำแหน่งที่ตั้งเหล่านี้อาจไม่ปลอดภัยในมุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="ebad4-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="ebad4-117">คุณสามารถอ่านแฟ้ม และดูเนื้อหาในขณะที่การลดความเสี่ยง โดยใช้มุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="ebad4-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="ebad4-118">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับมุมมองที่ได้รับการป้องกันและวิธีการเปลี่ยนการตั้งค่า ให้ดูที่บทความนี้:[มุมมองที่ได้รับการป้องกันคืออะไร?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="ebad4-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="ebad4-119">**OneDrive จะเต็มหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="ebad4-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="ebad4-120">ถ้าแฟ้มเก็บอยู่บน OneDrive และพื้นที่การจัดเก็บ OneDrive ของคุณจะเต็ม คุณจะไม่สามารถบันทึกเอกสารจนกว่าคุณจะอยู่ภายใต้พื้นที่ที่อนุญาตของคุณ</span><span class="sxs-lookup"><span data-stu-id="ebad4-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="ebad4-121">คุณสามารถตรวจสอบเนื้อที่ว่างของคุณบน OneDrive ได้ โดยคลิกไอคอน OneDrive ในศูนย์การแจ้งเตือน และเลือกจัดเก็บ หรือคุณยังสามารถไปที่[http://onedrive.live.com](http://onedrive.live.com)เข้าสู่ระบบ และหมายเหตุขนาดของเนื้อที่ที่ใช้ในหน้าต่างด้านล่างซ้ายของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="ebad4-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="ebad4-122">**เรียกใช้ Office ได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="ebad4-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="ebad4-123">ถ้าไม่มีการเปิดใช้งาน Office หรือสมัครใช้งานของคุณหมดอายุแล้ว คุณอาจเป็นในโหมดอ่านอย่างเดียวลดฟังก์ชันการทำงาน</span><span class="sxs-lookup"><span data-stu-id="ebad4-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="ebad4-124">สำหรับข้อมูลเกี่ยวกับวิธีการเปิดใช้งาน Office ดู:[ผลิตภัณฑ์สิทธิ์และข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="ebad4-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="ebad4-125">**ถ้าทั้งหมดล้มเหลว...**</span><span class="sxs-lookup"><span data-stu-id="ebad4-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="ebad4-126">ลองเริ่มการทำงานของคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="ebad4-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="ebad4-127">ติดตั้งโปรแกรมปรับปรุง Office</span><span class="sxs-lookup"><span data-stu-id="ebad4-127">Install Office updates</span></span>
    
- <span data-ttu-id="ebad4-128">การซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="ebad4-128">Perform an Online repair of Office</span></span>
    

