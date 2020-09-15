---
title: เริ่มต้นใช้งาน SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700726"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="5d77b-102">เวิร์กโฟลว์ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="5d77b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="5d77b-103">ถ้าเวิร์กโฟลว์ SharePoint ไม่ได้ส่งอีเมลองค์กรของคุณอาจพบข้อจำกัดของผู้ส่ง Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5d77b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="5d77b-104">ข้อความแสดงข้อผิดพลาด ' เวิร์กโฟลว์ is ถูกระงับ ' อาจเกิดขึ้นถ้าคุณมีหนึ่งในรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5d77b-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="5d77b-105">คุณมีเวิร์กโฟลว์ใน SharePoint Online ที่กำลังใช้ชนิดของแพลตฟอร์มเวิร์กโฟลว์ sharepoint ๒๐๑๐หรือ SharePoint ๒๐๑๓</span><span class="sxs-lookup"><span data-stu-id="5d77b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="5d77b-106">เวิร์กโฟลว์ถูกกำหนดค่าให้ส่งข้อความอีเมลที่กำหนดเองไปยังผู้ใช้มากกว่า๒๐๐คนในเวลามากกว่าผู้รับ๑๐,๐๐๐รายต่อวันหรือมากกว่า30ข้อความต่อนาที</span><span class="sxs-lookup"><span data-stu-id="5d77b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="5d77b-107">เมื่อคุณเรียกใช้เวิร์กโฟลว์ข้อความอีเมลจะไม่ถูกส่งและคุณสังเกตเห็นข้อความแสดงข้อผิดพลาดสถานะภายในถูกตั้งค่าเป็นหยุดชั่วคราวหรือไม่สามารถส่งไปยังผู้รับจะแสดงขึ้น</span><span class="sxs-lookup"><span data-stu-id="5d77b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="5d77b-108">สำหรับข้อมูลเพิ่มเติมโปรดดู [บทความ](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)ต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5d77b-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

