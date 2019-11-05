---
title: การป้องกันสแปม 5.4.1 DBEB จับทั้งหมด
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964347"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="393c4-102">แก้ไขปัญหาการจัดส่งสำหรับรหัสข้อผิดพลาด๕๕๐5.4.1 การเข้าถึงรีเลย์ถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="393c4-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="393c4-103">ปัญหานี้เกิดขึ้นเมื่อ[ตรวจสอบเพื่อดูว่าที่อยู่ e-mail ถูกต้องเพื่อป้องกันไม่ให้ bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)เมื่อเข้าสู่เครือข่าย Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="393c4-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="393c4-104">ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="393c4-104">Try the following:</span></span>

1. <span data-ttu-id="393c4-105">ตรวจสอบว่าปัญหามีความเฉพาะเจาะจงสำหรับทั้งโดเมนหรือที่อยู่เดียว:</span><span class="sxs-lookup"><span data-stu-id="393c4-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="393c4-106">โดเมนทั้งหมด: บางครั้งโดเมนต้องทำข้อมูลให้ตรงกัน ลอง[ตั้งค่าโดเมนเป็น "ภายใน" แล้วกลับไปที่](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="393c4-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="393c4-107">ที่อยู่เดียว: บางครั้งที่อยู่จะต้องมีการทำข้อมูลให้ตรงกัน การเปลี่ยนแปลงที่อยู่พร็อกซี smtp และจากนั้นเปลี่ยนกลับสามารถช่วย</span><span class="sxs-lookup"><span data-stu-id="393c4-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="393c4-108">ตรวจสอบว่าปัญหาที่เกิดขึ้นเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="393c4-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="393c4-109">วัตถุบางชนิดอาจต้องถูกสร้างด้วยตนเองในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="393c4-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="393c4-110">หากคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดตั๋วสนับสนุนและระบุขอบเขตของปัญหา (includidng ชนิดของวัตถุที่คุณกำลังส่งไป) เพื่อให้เราสามารถช่วยให้คุณได้ดียิ่งขึ้น</span><span class="sxs-lookup"><span data-stu-id="393c4-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>