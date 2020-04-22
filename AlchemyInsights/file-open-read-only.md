---
title: เปิดแฟ้มแบบอ่านอย่างเดียว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702793"
---
# <a name="file-open-read-only"></a><span data-ttu-id="bfa94-102">เปิดแฟ้มแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="bfa94-102">File open read-only</span></span>

<span data-ttu-id="bfa94-103">คุณอาจพบว่าเมื่อคุณกําลังเปิดแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="bfa94-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="bfa94-104">ในบางกรณี นี้คือการเพิ่มความปลอดภัย เช่น เมื่อคุณกําลังเปิดแฟ้มจากอินเทอร์เน็ต และบางครั้ง อาจเนื่องมาจากการตั้งค่าที่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="bfa94-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="bfa94-105">ต่อไปนี้เป็นบางสถานการณ์ที่แฟ้มเปิดอ่านได้อย่างเดียว และบางขั้นตอนที่คุณสามารถดําเนินการเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="bfa94-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="bfa94-106">**โปรแกรมป้องกันไวรัสของฉันเป็นสาเหตุให้พวกเขาเปิดแบบอ่านอย่างเดียว**</span><span class="sxs-lookup"><span data-stu-id="bfa94-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="bfa94-107">โปรแกรมป้องกันไวรัสบางโปรแกรมอาจป้องกันคุณจากแฟ้มที่อาจไม่ปลอดภัยด้วยการเปิดแฟ้มแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="bfa94-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="bfa94-108">คุณอาจต้องตรวจสอบกับผู้ให้บริการป้องกันไวรัสของคุณเพื่อเรียนรู้วิธีการปรับการตั้งค่าเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="bfa94-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="bfa94-109">ตัวอย่างเช่น BitDefender มีเนื้อหาเกี่ยวกับการเพิ่มข้อยกเว้นโปรแกรมที่นี่ :[วิธีการเพิ่มโปรแกรมหรือข้อยกเว้นกระบวนการในศูนย์ควบคุม](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="bfa94-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="bfa94-110">**คุณสมบัติแฟ้มถูกตั้งค่าเป็นอ่านอย่างเดียวหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="bfa94-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="bfa94-111">คุณสามารถตรวจสอบคุณสมบัติของแฟ้มโดยการคลิกขวาที่แฟ้มและเลือกคุณสมบัติ</span><span class="sxs-lookup"><span data-stu-id="bfa94-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="bfa94-112">ถ้าเลือกแอตทริบิวต์อ่านอย่างเดียวคุณสามารถยกเลิกการเลือกและคลิกตกลง</span><span class="sxs-lookup"><span data-stu-id="bfa94-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="bfa94-113">**เนื้อหาอยู่ในมุมมองที่ได้รับการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="bfa94-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="bfa94-114">ไฟล์จากอินเทอร์เน็ตและจากสถานที่ที่อาจไม่ปลอดภัยอื่น ๆ สามารถมีไวรัส เวิร์ม หรือมัลแวร์ชนิดอื่นที่อาจเป็นอันตรายต่อคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="bfa94-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="bfa94-115">นี่เป็นกรณีที่มีไฟล์แนบอีเมลหรือไฟล์ที่คุณดาวน์โหลดมา</span><span class="sxs-lookup"><span data-stu-id="bfa94-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="bfa94-116">แฟ้มจากตําแหน่งที่ตั้งที่อาจไม่ปลอดภัยเหล่านี้จะถูกเปิดในมุมมองที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="bfa94-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="bfa94-117">ด้วยการใช้มุมมองที่ได้รับการป้องกัน คุณสามารถอ่านแฟ้มและดูเนื้อหาของแฟ้มนั้นในขณะที่ลดความเสี่ยงได้</span><span class="sxs-lookup"><span data-stu-id="bfa94-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="bfa94-118">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับมุมมองที่ได้รับการป้องกันและวิธีการเปลี่ยนแปลงการตั้งค่า ให้ดูบทความนี้[: มุมมองที่ได้รับการป้องกันคืออะไร](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="bfa94-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="bfa94-119">**เต็มหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="bfa94-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="bfa94-120">ถ้าแฟ้มถูกจัดเก็บไว้บน OneDrive และพื้นที่เก็บข้อมูล OneDrive ของคุณเต็ม คุณจะไม่สามารถบันทึกเอกสารได้จนกว่าคุณจะอยู่ในพื้นที่ที่จัดสรรไว้</span><span class="sxs-lookup"><span data-stu-id="bfa94-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="bfa94-121">คุณสามารถตรวจสอบพื้นที่ว่างบน OneDrive ได้โดยคลิกไอคอน OneDrive ในศูนย์การแจ้งเตือน และเลือก จัดการพื้นที่จัดเก็บ หรือคุณสามารถไปที่[https://onedrive.live.com](https://onedrive.live.com)ลงชื่อเข้าใช้ และสังเกตจํานวนเนื้อที่ที่ใช้อยู่ด้านล่างซ้ายของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="bfa94-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="bfa94-122">**เปิดใช้งาน Office หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="bfa94-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="bfa94-123">ถ้า Office ไม่ได้เปิดใช้งาน หรือถ้าการสมัครใช้งานของคุณหมดอายุ คุณอาจอยู่ในโหมดลดฟังก์ชันการทํางานแบบอ่านอย่างเดียว</span><span class="sxs-lookup"><span data-stu-id="bfa94-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="bfa94-124">สําหรับข้อมูลเกี่ยวกับวิธีการเปิดใช้งาน Office ให้ดูที่:[ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="bfa94-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="bfa94-125">**ถ้าทั้งหมดอื่นล้มเหลว...**</span><span class="sxs-lookup"><span data-stu-id="bfa94-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="bfa94-126">ลองรีสตาร์ทคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="bfa94-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="bfa94-127">ติดตั้งโปรแกรมปรับปรุง Office</span><span class="sxs-lookup"><span data-stu-id="bfa94-127">Install Office updates</span></span>
    
- <span data-ttu-id="bfa94-128">ดําเนินการซ่อมแซมแบบออนไลน์ของ Office</span><span class="sxs-lookup"><span data-stu-id="bfa94-128">Perform an Online repair of Office</span></span>
    

