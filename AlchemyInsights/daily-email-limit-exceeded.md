---
title: เกินขีดจํากัดของอีเมลรายวัน เวิร์กโฟลว์ถูกระงับ
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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908723"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="8ca29-103">เกินขีดจํากัดอีเมลรายวันแล้ว</span><span class="sxs-lookup"><span data-stu-id="8ca29-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="8ca29-104">เวิร์กโฟลว์ถูกระงับ</span><span class="sxs-lookup"><span data-stu-id="8ca29-104">Workflow is suspended.</span></span>

<span data-ttu-id="8ca29-105">ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8ca29-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="8ca29-106">คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ชนิดแพลตฟอร์มเวิร์กโฟลว์ SharePoint 2010 หรือ SharePoint 2013</span><span class="sxs-lookup"><span data-stu-id="8ca29-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="8ca29-107">เวิร์กโฟลว์ถูกกําหนดค่าให้ส่งข้อความอีเมลแบบกําหนดเองไปยังผู้ใช้มากกว่า 200 คนในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="8ca29-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="8ca29-108">เมื่อคุณเรียกใช้เวิร์กโฟลว์ ข้อความอีเมลที่จะไม่ส่ง และคุณสังเกตเห็นลักษณะการทํางานต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8ca29-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="8ca29-109">สําหรับเวิร์กโฟลว์ที่ใช้ชนิดแพลตฟอร์ม SharePoint 2013 คุณเรียกดูไปยังหน้า**สถานะเวิร์กโฟลว์**</span><span class="sxs-lookup"><span data-stu-id="8ca29-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="8ca29-110">บนหน้า สถานะเวิร์กโฟลว์**สถานะภายใน**ถูกตั้งค่าเป็น**เริ่มต้น**แล้ว และบอลลูนข้อมูลจะแสดง**ไม่สามารถส่งไปยังผู้รับ**ได้</span><span class="sxs-lookup"><span data-stu-id="8ca29-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="8ca29-111">เมื่อต้องการหลีกเลี่ยงปัญหานี้ กําหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความอีเมลโดยไม่เกิน[ขีดจํากัดผู้ส่งแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)</span><span class="sxs-lookup"><span data-stu-id="8ca29-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="8ca29-112">ตัวอย่างเช่น ใช้หยุดชั่วคราวในเวิร์กโฟลว์ ส่งอีเมลไปยังกลุ่ม Microsoft 365 กลุ่มการแจกจ่ายหรือกลุ่มรักษาความปลอดภัยที่เปิดใช้งานจดหมาย หรือส่งข้อความไปยังผู้รับน้อยกว่า 200 ในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="8ca29-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="8ca29-113">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="8ca29-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="8ca29-114">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="8ca29-114">Related topics</span></span>
- [<span data-ttu-id="8ca29-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="8ca29-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8ca29-116">SharePoint และโฟลว์</span><span class="sxs-lookup"><span data-stu-id="8ca29-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 