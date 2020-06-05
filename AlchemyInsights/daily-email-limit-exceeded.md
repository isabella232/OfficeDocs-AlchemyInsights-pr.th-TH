---
title: เกินขีดจํากัดอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580352"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="6bb0d-103">เกินขีดจํากัดอีเมลรายวัน</span><span class="sxs-lookup"><span data-stu-id="6bb0d-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="6bb0d-104">เวิร์กโฟลว์ถูกระงับ</span><span class="sxs-lookup"><span data-stu-id="6bb0d-104">Workflow is suspended.</span></span>

<span data-ttu-id="6bb0d-105">ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6bb0d-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="6bb0d-106">คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ชนิดแพลตฟอร์มลําดับงาน SharePoint 2010 หรือ SharePoint 2013</span><span class="sxs-lookup"><span data-stu-id="6bb0d-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="6bb0d-107">เวิร์กโฟลว์ถูกกําหนดค่าให้ส่งข้อความอีเมลที่กําหนดเองไปยังผู้ใช้มากกว่า 200 รายในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="6bb0d-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="6bb0d-108">เมื่อคุณเรียกใช้เวิร์กโฟลว์ ข้อความอีเมลที่ไม่ได้ส่ง และคุณสังเกตเห็นลักษณะการทํางานต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6bb0d-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="6bb0d-109">สําหรับเวิร์กโฟลว์ที่ใช้ชนิดแพลตฟอร์ม SharePoint 2013 คุณเรียกดูไปยังหน้า**สถานะเวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="6bb0d-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="6bb0d-110">บนหน้า สถานะเวิร์กโฟลว์**สถานะภายใน**จะถูกตั้งค่าเป็น**เริ่มต้น**แล้วบอลลูนข้อมูลจะแสดง**ไม่สามารถส่งไปยังผู้รับ**ได้</span><span class="sxs-lookup"><span data-stu-id="6bb0d-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="6bb0d-111">เมื่อต้องการหลีกเลี่ยงปัญหานี้ ให้กําหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่มีการ[เกินขีดจํากัดของผู้ส่ง Exchange แบบออนไลน์](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)</span><span class="sxs-lookup"><span data-stu-id="6bb0d-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="6bb0d-112">ตัวอย่างเช่น ใช้การหยุดชั่วคราวในเวิร์กโฟลว์ ส่งอีเมลไปยังกลุ่ม Microsoft 365 กลุ่มการแจกจ่ายหรือจดหมายที่เปิดใช้งานกลุ่มรักษาความปลอดภัย หรือส่งข้อความไปยังผู้รับน้อยกว่า 200 ครั้ง</span><span class="sxs-lookup"><span data-stu-id="6bb0d-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="6bb0d-113">สําหรับข้อมูลเพิ่มเติม ให้ดู[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="6bb0d-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6bb0d-114">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="6bb0d-114">Related topics</span></span>
- [<span data-ttu-id="6bb0d-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="6bb0d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6bb0d-116">การไหลและจุด</span><span class="sxs-lookup"><span data-stu-id="6bb0d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 