---
title: แอนตี้สแปม-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717344"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="3bbb8-102">แก้ไขปัญหาการนำส่งอีเมลสำหรับรหัสข้อผิดพลาด5.7.23</span><span class="sxs-lookup"><span data-stu-id="3bbb8-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="3bbb8-103">ตรวจสอบระเบียน DNS ของ SPF สำหรับโดเมนของคุณที่มีตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานสาธารณะบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="3bbb8-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="3bbb8-104">ตรวจสอบว่าข้อความขาออกจะไม่ถูกระบุว่าเป็นสแปมโดย Microsoft และกำหนดเส้นทางผ่านทางกลุ่มการนำ[ส่งความเสี่ยงสูง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="3bbb8-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="3bbb8-105">ข้อความในกลุ่มการนำส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจึงไม่ได้รับการยอมรับจากองค์กรอีเมลของปลายทาง</span><span class="sxs-lookup"><span data-stu-id="3bbb8-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="3bbb8-106">ถ้าปัญหายังคงมีอยู่คุณอาจจำเป็นต้องติดต่อผู้ดูแลระบบของ host mail ที่คุณกำลังพยายามส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="3bbb8-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="3bbb8-107">จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่พร้อมใช้งานในข้อความตีกลับ</span><span class="sxs-lookup"><span data-stu-id="3bbb8-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="3bbb8-108">ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="3bbb8-108">Microsoft support may not be able to assist further.</span></span>
