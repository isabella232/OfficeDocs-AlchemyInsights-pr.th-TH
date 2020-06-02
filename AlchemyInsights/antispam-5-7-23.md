---
title: ป้องกันโรคไข้ - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506462"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="5b11e-102">แก้ไขปัญหาการนําส่งอีเมลสําหรับรหัสข้อผิดพลาด 5.7.23</span><span class="sxs-lookup"><span data-stu-id="5b11e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="5b11e-103">ตรวจสอบระเบียน DNS SPF สําหรับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานแบบสาธารณะบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="5b11e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="5b11e-104">ตรวจสอบว่า ข้อความขาออกไม่ได้ถูกระบุว่าเป็นสแปม โดย Microsoft และกําหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="5b11e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="5b11e-105">ข้อความในพูลการจัดส่งที่มีความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และองค์กรอีเมลปลายทางจะไม่ได้รับการยอมรับ</span><span class="sxs-lookup"><span data-stu-id="5b11e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="5b11e-106">หากปัญหายังคงมีอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์อีเมลที่คุณกําลังพยายามส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="5b11e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="5b11e-107">จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดในข้อความตีกลับ</span><span class="sxs-lookup"><span data-stu-id="5b11e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="5b11e-108">การสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="5b11e-108">Microsoft support may not be able to assist further.</span></span>
