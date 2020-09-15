---
title: แอนตี้สแปม 5.4.1 DBEB
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717380"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ea4df-102">แก้ไขปัญหาการนำส่งสำหรับรหัสข้อผิดพลาด๕๕๐5.4.1 การเข้าถึงรีเลย์ที่ถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="ea4df-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ea4df-103">ปัญหานี้เกิดขึ้นเมื่อ [ตรวจสอบเพื่อดูว่าที่อยู่อีเมลไม่ถูกต้องในการป้องกันไม่ให้ bouncebacks เมื่อเข้า](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) สู่เครือข่าย Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea4df-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ea4df-104">ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ea4df-104">Try the following:</span></span>

1. <span data-ttu-id="ea4df-105">ตรวจสอบว่าปัญหาเฉพาะกับโดเมนทั้งหมดหรือที่อยู่อีเมลเดียว:</span><span class="sxs-lookup"><span data-stu-id="ea4df-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ea4df-106">โดเมนทั้งหมด: บางครั้งจำเป็นต้องซิงโครไนซ์โดเมน ลอง[ตั้งค่าโดเมนเป็นภายในแล้วกลับไปยังสิทธิ์](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="ea4df-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ea4df-107">อีเมลแอดเดรสเดียว: บางครั้งจำเป็นต้องซิงโครไนซ์ที่อยู่ การเปลี่ยนที่อยู่พร็อกซีของ smtp แล้วการเปลี่ยนกลับจะช่วยให้คุณสามารถช่วยได้</span><span class="sxs-lookup"><span data-stu-id="ea4df-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ea4df-108">ตรวจสอบว่าปัญหาเฉพาะกับกลุ่มหรือโฟลเดอร์สาธารณะหรือไม่</span><span class="sxs-lookup"><span data-stu-id="ea4df-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ea4df-109">สำหรับชนิดของวัตถุบางชนิดวัตถุอาจจำเป็นต้องถูกสร้างขึ้นด้วยตนเองใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ea4df-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ea4df-110">ถ้าคุณต้องการความช่วยเหลือเพิ่มเติมโปรดเปิดบัตรสนับสนุนและระบุขอบเขตของปัญหา (รวมถึงชนิดของวัตถุที่คุณกำลังส่งไป) เพื่อให้เราสามารถช่วยคุณได้ดียิ่งขึ้น</span><span class="sxs-lookup"><span data-stu-id="ea4df-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>