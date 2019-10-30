---
title: เริ่มต้นใช้งาน SharePoint แบบออนไลน์
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766910"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="9e162-102">เวิร์กโฟลว์ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="9e162-102">Workflows in SharePoint</span></span>

<span data-ttu-id="9e162-103">ถ้าเวิร์กโฟลว์ SharePoint จะไม่ส่งเมลองค์กรของคุณอาจพบข้อจำกัดของผู้ส่งการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="9e162-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="9e162-104">ข้อความข้อผิดพลาด ' เวิร์กโฟลว์ถูกระงับ ' อาจเกิดขึ้นได้หากคุณมีหนึ่งในรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9e162-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="9e162-105">คุณมีเวิร์กโฟลว์ใน SharePoint แบบออนไลน์ที่ใช้ SharePoint ๒๐๑๐หรือ SharePoint ๒๐๑๓ชนิดแพลตฟอร์มเวิร์กโฟลว์</span><span class="sxs-lookup"><span data-stu-id="9e162-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="9e162-106">เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความเมลแบบกำหนดเองไปยังผู้ใช้มากกว่า๒๐๐ในแต่ละครั้งมากกว่า๑๐,๐๐๐ผู้รับต่อวันหรือมากกว่า30ข้อความต่อนาที</span><span class="sxs-lookup"><span data-stu-id="9e162-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="9e162-107">เมื่อคุณเรียกใช้เวิร์กโฟลว์ไม่ได้ส่งข้อความจดหมายและคุณสังเกตเห็นข้อผิดพลาดสถานะภายในถูกตั้งค่าเป็นระงับหรือไม่สามารถส่งไปยังผู้รับจะแสดงขึ้น</span><span class="sxs-lookup"><span data-stu-id="9e162-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="9e162-108">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[บทความ](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="9e162-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

