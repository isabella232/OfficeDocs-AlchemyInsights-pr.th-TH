---
title: 1332 OWA - กฎของกล่องขาเข้าจะไม่ดำเนินการสำหรับกล่องจดหมาย
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784360"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="fb32e-102">กฎของกล่องขาเข้าไม่ทำงานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="fb32e-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="fb32e-103">ตรวจสอบการตั้งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fb32e-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="fb32e-104">ข้อความสามารถถูกเปลี่ยนเส้นทาง ส่งต่อ หรือโดยอัตโนมัติขึ้นอยู่กับกฎของกล่องขาเข้าเพียงครั้งเดียวเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="fb32e-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="fb32e-105">กฎการเปลี่ยนทิศทาง (ผิดกฎของกล่องขาเข้าหรือกระแสกฎสำหรับจดหมาย หรือที่เรียกอีกอย่างหนึ่งว่ากฎการขนส่ง) สามารถเพิ่มได้สูงสุดสิบการผู้รับส่งต่อข้อความ</span><span class="sxs-lookup"><span data-stu-id="fb32e-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="fb32e-106">สำหรับข้อมูลเพิ่มเติม ให้ดู[สมุดรายวัน ขน ส่ง และอินบ็อกซ์ขีดจำกัดกฎ](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)</span><span class="sxs-lookup"><span data-stu-id="fb32e-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="fb32e-107">กฎของกล่องขาเข้าไม่ทำงานกับกล่องจดหมายอื่นบันทึกนั้น</span><span class="sxs-lookup"><span data-stu-id="fb32e-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="fb32e-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายบันทึกสำรอง ดู[กล่องจดหมายบันทึกสำรอง](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)</span><span class="sxs-lookup"><span data-stu-id="fb32e-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="fb32e-109">เมื่อต้องการแก้ไขปัญหาเหล่านี้ ดู[KB 2829319](https://support.microsoft.com/kb/2829319)</span><span class="sxs-lookup"><span data-stu-id="fb32e-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="fb32e-110">ถ้าไม่สามารถใช้กับปัญหาก่อนหน้านี้ เรียกใช้การวินิจฉัยรายงานกฎกล่องขาเข้าก่อนที่คุณเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของ Microsoft:</span><span class="sxs-lookup"><span data-stu-id="fb32e-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="fb32e-111">เปิดกล่องจดหมายใน Outlook บนเว็บ และคลิกการ**ตั้งค่า** \> **ตัวเลือก** \> **จัดระเบียบอี** \> **กฎของกล่องขาเข้า**</span><span class="sxs-lookup"><span data-stu-id="fb32e-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="fb32e-112">ที่ด้านล่างของหน้า คลิก**ถ้ากฎของคุณกำลังทำงานอยู่ให้คลิกที่นี่เพื่อสร้างรายงานการวินิจฉัย**</span><span class="sxs-lookup"><span data-stu-id="fb32e-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

