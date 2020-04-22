---
title: ป้องกันสแปม 5.4.1 DBEB จับทั้งหมด
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707930"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="1f5dc-102">แก้ไขปัญหาการจัดส่งสําหรับรหัสข้อผิดพลาด 550 5.4.1 Relay Access ถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="1f5dc-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="1f5dc-103">ปัญหานี้เกิดขึ้นเมื่อ[ตรวจสอบเพื่อดูว่า อยู่อีเมลถูกต้องเพื่อป้องกัน bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)เมื่อเข้าสู่เครือข่ายของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="1f5dc-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="1f5dc-104">ลองทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="1f5dc-104">Try the following:</span></span>

1. <span data-ttu-id="1f5dc-105">ตรวจสอบว่า ปัญหาเฉพาะกับโดเมนทั้งหมดหรือที่อยู่อีเมลเดียว:</span><span class="sxs-lookup"><span data-stu-id="1f5dc-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="1f5dc-106">โดเมนทั้งหมด: บางครั้งโดเมนต้องถูกซิงโครไนซ์ ลอง[ตั้งค่าโดเมนเป็นภายในแล้วกลับไปที่ Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="1f5dc-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="1f5dc-107">ที่อยู่อีเมลเดียว: บางครั้งที่อยู่จะต้องมีการซิงโครไนซ์ การเปลี่ยนที่อยู่พร็อกซี SMTP แล้วเปลี่ยนกลับสามารถช่วย</span><span class="sxs-lookup"><span data-stu-id="1f5dc-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="1f5dc-108">ตรวจสอบว่า ปัญหาเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="1f5dc-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="1f5dc-109">สําหรับบางชนิดวัตถุ วัตถุอาจจําเป็นต้องถูกสร้างด้วยตนเองในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="1f5dc-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="1f5dc-110">หากคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดตั๋วสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงประเภทของวัตถุที่คุณกําลังส่งไป) เพื่อให้เราสามารถช่วยให้คุณดีขึ้น</span><span class="sxs-lookup"><span data-stu-id="1f5dc-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>