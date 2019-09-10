---
title: แฟ้มเปิดแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822253"
---
# <a name="file-open-read-only"></a><span data-ttu-id="987ee-102">แฟ้มเปิดแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="987ee-102">File open read-only</span></span>

<span data-ttu-id="987ee-103">คุณอาจพบว่าเมื่อคุณกำลังเปิดแฟ้มพวกเขาเปิดเป็นแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="987ee-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="987ee-104">ในบางกรณีนี้สำหรับการรักษาความปลอดภัยที่เพิ่มเข้ามาเช่นเมื่อคุณกำลังเปิดแฟ้มจากอินเทอร์เน็ตและเวลาอื่นๆอาจเกิดจากการตั้งค่าที่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="987ee-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="987ee-105">ต่อไปนี้เป็นบางสถานการณ์ที่แฟ้มเปิดแบบอ่านอย่างเดียวและบางขั้นตอนที่คุณสามารถดำเนินการเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="987ee-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="987ee-106">**โปรแกรมป้องกันไวรัสของฉันเป็นสาเหตุให้พวกเขาเปิดแบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="987ee-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="987ee-107">บางโปรแกรมป้องกันไวรัสอาจป้องกันคุณจากแฟ้มที่อาจไม่ปลอดภัยโดยการเปิดแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="987ee-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="987ee-108">คุณอาจต้องตรวจสอบกับผู้ให้บริการโปรแกรมป้องกันไวรัสของคุณเพื่อเรียนรู้วิธีการปรับการตั้งค่าเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="987ee-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="987ee-109">ตัวอย่างเช่น, มีเนื้อหาเกี่ยวกับการเพิ่มการยกเว้นแอพลิเคชันที่นี่:[วิธีการเพิ่มการประยุกต์ใช้หรือกระบวนการยกเว้นในศูนย์ควบคุม Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="987ee-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="987ee-110">**มีการตั้งค่าคุณสมบัติของแฟ้มเป็นแบบอ่านอย่างเดียวหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="987ee-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="987ee-111">คุณสามารถตรวจสอบคุณสมบัติของแฟ้มได้ด้วยการคลิกขวาที่แฟ้มแล้วเลือกคุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="987ee-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="987ee-112">ถ้ามีการตรวจสอบคุณลักษณะอ่านอย่างเดียวคุณสามารถยกเลิกการเลือกและคลิกตกลง</span><span class="sxs-lookup"><span data-stu-id="987ee-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="987ee-113">**เนื้อหาอยู่ในมุมมองที่ได้รับการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="987ee-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="987ee-114">แฟ้มจากอินเทอร์เน็ตและจากตำแหน่งที่ตั้งที่อาจไม่ปลอดภัยอื่นๆอาจมีไวรัสเวิร์มหรือมัลแวร์ชนิดอื่นๆที่อาจเป็นอันตรายต่อคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="987ee-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="987ee-115">นอกจากนี้ยังมักจะเป็นกรณีที่มีสิ่งที่แนบมากับ e-mail หรือไฟล์ที่คุณดาวน์โหลด</span><span class="sxs-lookup"><span data-stu-id="987ee-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="987ee-116">เพื่อช่วยป้องกันคอมพิวเตอร์ของคุณแฟ้มจากตำแหน่งที่ตั้งที่อาจไม่ปลอดภัยเหล่านี้จะถูกเปิดในมุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="987ee-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="987ee-117">โดยการใช้ ' มุมมองที่ได้รับการป้องกัน ' คุณสามารถอ่านแฟ้มและดูเนื้อหาในขณะที่ลดความเสี่ยงได้</span><span class="sxs-lookup"><span data-stu-id="987ee-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="987ee-118">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับมุมมองที่ได้รับการป้องกันและวิธีการเปลี่ยนการตั้งค่าโปรดดูบทความนี้:[มุมมองที่ได้รับการป้องกันคืออะไร](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="987ee-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="987ee-119">**เป็น OneDrive เต็มหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="987ee-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="987ee-120">ถ้าไฟล์ถูกเก็บไว้ใน OneDrive และพื้นที่จัดเก็บข้อมูล OneDrive ของคุณเต็มคุณจะไม่สามารถบันทึกเอกสารจนกว่าคุณจะอยู่ภายใต้พื้นที่ที่กำหนดของคุณ</span><span class="sxs-lookup"><span data-stu-id="987ee-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="987ee-121">คุณสามารถตรวจสอบพื้นที่ว่างของคุณบน OneDrive ได้โดยคลิกที่ไอคอน OneDrive ในศูนย์การแจ้งเตือนและเลือกจัดการพื้นที่จัด[http://onedrive.live.com](http://onedrive.live.com)เก็บข้อมูลหรือคุณสามารถไปที่ลงชื่อเข้าใช้และจดบันทึกจำนวนพื้นที่ที่ใช้ในด้านซ้ายล่างของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="987ee-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="987ee-122">**เปิดใช้งาน Office หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="987ee-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="987ee-123">ถ้า Office ไม่ได้เปิดใช้งานหรือถ้าการสมัครสมาชิกของคุณหมดอายุคุณอาจอยู่ในโหมดลดฟังก์ชันการทำงานแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="987ee-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="987ee-124">สำหรับข้อมูลเกี่ยวกับวิธีการเปิดใช้งาน Office ดู:[ข้อผิดพลาดของผลิตภัณฑ์และการเปิดใช้งานใน Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="987ee-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="987ee-125">**ถ้าทุกอย่างอื่นล้มเหลว**</span><span class="sxs-lookup"><span data-stu-id="987ee-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="987ee-126">ลองเริ่มระบบของคอมพิวเตอร์ใหม่</span><span class="sxs-lookup"><span data-stu-id="987ee-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="987ee-127">ติดตั้งโปรแกรมปรับปรุง Office</span><span class="sxs-lookup"><span data-stu-id="987ee-127">Install Office updates</span></span>
    
- <span data-ttu-id="987ee-128">ดำเนินการซ่อมแซมของ Office แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="987ee-128">Perform an Online repair of Office</span></span>
    

