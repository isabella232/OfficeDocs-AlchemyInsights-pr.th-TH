---
title: คำแนะนำด้านความปลอดภัยสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658134"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="0ba80-102">คำแนะนำด้านความปลอดภัยสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="0ba80-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="0ba80-p101">ถ้าคุณกำลัง รับเคล็ดลับความปลอดภัยที่บอกว่า "ผู้ส่งล้มเหลวเช็คของเราตรวจหาการฉ้อโกง และอาจไม่สามารถที่ จะปรากฏเป็น" จาก นั้นผู้ส่งไม่สามารถผ่านการตรวจสอบการรับรองความถูกต้องเป็น DKIM หรือ SPF การแก้ปัญหานี้เป็นวิธีดีสำหรับผู้ส่งเพื่ออนุมัติด้วยตนเองได้ ถ้าผู้ส่งกำลังส่งในนามของคุณ คุณจำเป็นต้องให้สิทธิ์ดังกล่าว โดยเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ</span><span class="sxs-lookup"><span data-stu-id="0ba80-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="0ba80-106">ดู[คำแนะนำด้านความปลอดภัย (น่าสงสัย) สีแดงสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="0ba80-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="0ba80-107">ต่อไปนี้เป็นบางลิงค์อื่น ๆ ที่สามารถช่วยให้:</span><span class="sxs-lookup"><span data-stu-id="0ba80-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="0ba80-108">วิธีที่ Office 365 ใช้โครงสร้างนโยบายของผู้ส่ง (SPF) เพื่อป้องกันการเคลื่อนย้าย</span><span class="sxs-lookup"><span data-stu-id="0ba80-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="0ba80-109">ตั้งค่า SPF ใน Office 365 เมื่อต้องการป้องกันการเคลื่อนย้าย</span><span class="sxs-lookup"><span data-stu-id="0ba80-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

