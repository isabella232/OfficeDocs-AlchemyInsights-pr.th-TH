---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821430"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="10d75-102">แก้ไขปัญหาการส่งอีเมลของรหัสข้อผิดพลาด 5.7.23</span><span class="sxs-lookup"><span data-stu-id="10d75-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="10d75-103">ตรวจสอบระเบียน DNS ของ SPF กับโดเมนของคุณที่ตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานแบบสาธารณะบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="10d75-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="10d75-104">ตรวจสอบว่าข้อความขาออกไม่ได้ระบุว่าเป็นสแปมโดยไมโครซอฟท์ และถูกเส้นทางผ่าน [พูลการส่งข้อความความเสี่ยง](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)สูง</span><span class="sxs-lookup"><span data-stu-id="10d75-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="10d75-105">ข้อความในพูลการส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF ดังนั้นจึงไม่ได้รับการยอมรับจากองค์กรอีเมลปลายทาง</span><span class="sxs-lookup"><span data-stu-id="10d75-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="10d75-106">ถ้าปัญหายังคงอยู่ คุณอาจต้องติดต่อผู้ดูแลระบบของโฮสต์จดหมายที่คุณพยายามส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="10d75-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="10d75-107">จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่พร้อมใช้งานในข้อความแจ้งการตีกลับ</span><span class="sxs-lookup"><span data-stu-id="10d75-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="10d75-108">ฝ่ายสนับสนุนของ Microsoft อาจไม่สามารถช่วยเหลือเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="10d75-108">Microsoft support may not be able to assist further.</span></span>
