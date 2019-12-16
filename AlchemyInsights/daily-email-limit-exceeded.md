---
title: เกินขีดจำกัดของ email รายวัน เวิร์กโฟลว์ถูกระงับ
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053136"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="e86cd-103">เกินขีดจำกัดของ email รายวัน</span><span class="sxs-lookup"><span data-stu-id="e86cd-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="e86cd-104">เวิร์กโฟลว์ถูกระงับ</span><span class="sxs-lookup"><span data-stu-id="e86cd-104">Workflow is suspended.</span></span>

<span data-ttu-id="e86cd-105">ข้อผิดพลาดนี้อาจได้รับในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e86cd-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="e86cd-106">คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ SharePoint ๒๐๑๐หรือ SharePoint ๒๐๑๓ชนิดแพลตฟอร์มเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="e86cd-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="e86cd-107">เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความเมลแบบกำหนดเองไปยังผู้ใช้มากกว่า๒๐๐ในแต่ละครั้งมากกว่า๑๐,๐๐๐ผู้รับต่อวันหรือมากกว่า30ข้อความต่อนาที</span><span class="sxs-lookup"><span data-stu-id="e86cd-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="e86cd-108">เมื่อคุณเรียกใช้เวิร์กโฟลว์ข้อความทางเมลไม่ถูกส่งและคุณสังเกตเห็นลักษณะการทำงานต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e86cd-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="e86cd-109">สำหรับเวิร์กโฟลว์โดยใช้ชนิดแพลตฟอร์ม SharePoint ๒๐๑๓คุณเรียกดูไปยังหน้า**สถานะลำดับงาน**</span><span class="sxs-lookup"><span data-stu-id="e86cd-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="e86cd-110">บนหน้าสถานะลำดับงาน**สถานะภายใน**ถูกตั้งค่าเป็น**เริ่มต้น**และบอลลูนข้อมูลแสดง**ไม่สามารถส่งไปยังผู้รับ**</span><span class="sxs-lookup"><span data-stu-id="e86cd-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="e86cd-111">การกำหนดค่าเวิร์กโฟลว์ของคุณเพื่อส่งข้อความทางเมลโดยไม่เกิน[ขีดจำกัดผู้ส่งแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)</span><span class="sxs-lookup"><span data-stu-id="e86cd-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="e86cd-112">ตัวอย่างเช่นใช้หยุดการทำงานในเวิร์กโฟลว์ให้ส่งจดหมายไปยังกลุ่ม Office ๓๖๕, กลุ่มการแจกจ่ายหรือกลุ่มรักษาความปลอดภัยที่เปิดใช้งานเมลหรือส่งข้อความไปยังผู้รับน้อยกว่า๒๐๐ในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="e86cd-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="e86cd-113">สำหรับข้อมูลเพิ่มเติมให้ดู[บทความ](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="e86cd-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="e86cd-114">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="e86cd-114">Related topics</span></span>
- [<span data-ttu-id="e86cd-115">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="e86cd-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e86cd-116">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="e86cd-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 