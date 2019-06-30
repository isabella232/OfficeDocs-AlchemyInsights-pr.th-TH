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
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353268"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c5e94-102">คำแนะนำด้านความปลอดภัยสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="c5e94-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c5e94-103">ถ้าคุณกำลัง รับเคล็ดลับความปลอดภัยที่บอกว่า "ผู้ส่งล้มเหลวเช็คของเราตรวจหาการฉ้อโกง และอาจไม่สามารถที่ จะปรากฏเป็น" จาก นั้นผู้ส่งไม่สามารถผ่านการตรวจสอบการรับรองความถูกต้องเป็น DKIM หรือ SPF</span><span class="sxs-lookup"><span data-stu-id="c5e94-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c5e94-104">การแก้ปัญหานี้เป็นวิธีดีสำหรับผู้ส่งเพื่ออนุมัติด้วยตนเองได้</span><span class="sxs-lookup"><span data-stu-id="c5e94-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c5e94-105">ถ้าผู้ส่งกำลังส่งในนามของคุณ คุณจำเป็นต้องให้สิทธิ์ดังกล่าว โดยเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5e94-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c5e94-106">ดู[คำแนะนำด้านความปลอดภัย (น่าสงสัย) สีแดงสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="c5e94-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c5e94-107">ต่อไปนี้เป็นบางลิงค์อื่น ๆ ที่สามารถช่วยให้:</span><span class="sxs-lookup"><span data-stu-id="c5e94-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c5e94-108">วิธีที่ Office 365 ใช้โครงสร้างนโยบายของผู้ส่ง (SPF) เพื่อป้องกันการเคลื่อนย้าย</span><span class="sxs-lookup"><span data-stu-id="c5e94-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c5e94-109">ตั้งค่า SPF ใน Office 365 เมื่อต้องการป้องกันการเคลื่อนย้าย</span><span class="sxs-lookup"><span data-stu-id="c5e94-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
