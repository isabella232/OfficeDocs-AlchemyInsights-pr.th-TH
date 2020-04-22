---
title: ป้องกันสแปม - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676516"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="7de82-102">แก้ไขปัญหาการนําส่งอีเมลสําหรับรหัสข้อผิดพลาด 5.7.23</span><span class="sxs-lookup"><span data-stu-id="7de82-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="7de82-103">ตรวจสอบระเบียน Dns SPF สําหรับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่มีอยู่สาธารณะบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="7de82-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="7de82-104">ตรวจสอบว่า ข้อความขาออกไม่ได้ถูกระบุว่าเป็นสแปมโดย Microsoft และกําหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="7de82-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="7de82-105">ข้อความในพูลการส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจะไม่ได้รับการยอมรับโดยองค์กรอีเมลปลายทาง</span><span class="sxs-lookup"><span data-stu-id="7de82-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="7de82-106">หากปัญหายังคงมีอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์อีเมลที่คุณกําลังพยายามส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="7de82-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="7de82-107">จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่มีอยู่ในข้อความตีกลับ</span><span class="sxs-lookup"><span data-stu-id="7de82-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="7de82-108">ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถให้ความช่วยเหลือเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="7de82-108">Microsoft support may not be able to assist further.</span></span>
