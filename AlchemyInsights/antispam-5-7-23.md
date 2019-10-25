---
title: การป้องกันสแปม-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682326"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f4700-102">แก้ไขปัญหาการส่งเมล์สำหรับรหัสข้อผิดพลาด5.7.23</span><span class="sxs-lookup"><span data-stu-id="f4700-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f4700-103">ตรวจสอบระเบียน SPF DNS สำหรับโดเมนของคุณในตัวตรวจสอบระเบียน SPF หรือ DNS ที่พร้อมใช้งานสาธารณะบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="f4700-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f4700-104">ตรวจสอบว่าข้อความขาออกไม่ได้ระบุว่าเป็นสแปมโดย Office ๓๖๕และกำหนดเส้นทางผ่าน[กลุ่มการจัดส่งความเสี่ยงสูง](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="f4700-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f4700-105">ข้อความในพูลการจัดส่งความเสี่ยงสูงจะไม่ผ่านการตรวจสอบ SPF และดังนั้นจึงจะไม่ได้รับการอนุญาตจากองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="f4700-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f4700-106">ถ้าปัญหายังคงมีอยู่คุณอาจต้องติดต่อผู้ดูแลของโฮสต์จดหมายที่คุณกำลังพยายามที่จะส่งทางเมล</span><span class="sxs-lookup"><span data-stu-id="f4700-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f4700-107">จดบันทึกข้อผิดพลาดภายนอกโดยละเอียดที่มีอยู่ในข้อความตีกลับ</span><span class="sxs-lookup"><span data-stu-id="f4700-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="f4700-108">การสนับสนุน Office ๓๖๕อาจไม่สามารถช่วยเหลือเพิ่มเติมได้</span><span class="sxs-lookup"><span data-stu-id="f4700-108">Office 365 support may not be able to assist further.</span></span>