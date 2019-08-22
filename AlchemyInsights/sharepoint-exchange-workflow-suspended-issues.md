---
title: เริ่มต้นใช้งาน SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: ae27a9fc342eb4fc4633ffd5518d63600b978db8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504014"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ab12b-102">เวิร์กโฟลว์ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="ab12b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ab12b-103">ถ้าเวิร์กโฟลว์ SharePoint ไม่ได้กำลังส่งอีเมล์ องค์กรของคุณอาจจะพบขีดจำกัดผู้ส่งอัตราแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ab12b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ab12b-104">ข้อความแสดงข้อผิดพลาด 'ลำดับงานหยุดการทำงาน' จะเกิดขึ้นถ้าคุณมีตัวเลือกอย่างใดอย่างหนึ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ab12b-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ab12b-105">คุณมีลำดับงานใน SharePoint แบบออนไลน์ที่กำลังใช้ SharePoint 2010 หรือชนิดแพลตฟอร์มเวิร์กโฟลว์ SharePoint 2013 ในส่วน</span><span class="sxs-lookup"><span data-stu-id="ab12b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ab12b-106">เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความอีเมลที่กำหนดเองแก่ผู้ใช้มากกว่า 200 ในแต่ละครั้ง ผู้รับมากกว่า 10000 ต่อวัน หรือข้อความมากกว่า 30 ต่อนาที</span><span class="sxs-lookup"><span data-stu-id="ab12b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ab12b-107">เมื่อคุณเรียกใช้เวิร์กโฟลว์ ไม่ได้ส่งข้อความอีเมล และคุณพบข้อผิดพลาด ภายในสถานะถูกตั้งค่าเป็นระงับหรือไม่เมื่อต้องการส่งไปยังผู้รับจะแสดงขึ้น</span><span class="sxs-lookup"><span data-stu-id="ab12b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ab12b-108">สำหรับข้อมูลเพิ่มเติม โปรดดูที่[บท](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)ความต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="ab12b-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

