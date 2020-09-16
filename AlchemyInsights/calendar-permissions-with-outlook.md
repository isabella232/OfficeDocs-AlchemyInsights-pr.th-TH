---
title: สิทธิ์ของปฏิทิน
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748812"
---
# <a name="calendar-permissions"></a><span data-ttu-id="2de44-102">สิทธิ์ของปฏิทิน</span><span class="sxs-lookup"><span data-stu-id="2de44-102">Calendar Permissions</span></span>

<span data-ttu-id="2de44-103">ผู้ใช้สามารถเปลี่ยนแปลงสิทธิ์ของปฏิทินของตนเองกับ Outlook บนเว็บหรือไคลเอ็นต์อื่นๆได้แต่เป็นผู้ดูแลระบบที่คุณอาจต้องการตรวจสอบด้วยเช่นกัน</span><span class="sxs-lookup"><span data-stu-id="2de44-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="2de44-104">ด้วย cmdlet PowerShell Exchange จะแสดงสิทธิ์ในปฏิทินของผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="2de44-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="2de44-105">เมื่อต้องการดูข้อมูลเพิ่มเติมให้ดูที่ข้อมูลต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="2de44-105">To see more information see the following:</span></span>

- [<span data-ttu-id="2de44-106">รับ-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="2de44-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2de44-107">ตั้งค่า-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="2de44-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2de44-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="2de44-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="2de44-109">สิทธิ์ของปฏิทินจะถูกใช้ในการแชร์ปฏิทินเพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการแชร์ปฏิทิน Outlook ให้ดูบทความเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="2de44-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="2de44-110">แชร์ปฏิทิน Outlook กับบุคคลอื่น</span><span class="sxs-lookup"><span data-stu-id="2de44-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="2de44-111">แชร์ปฏิทินของคุณใน Outlook บนเว็บสำหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="2de44-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="2de44-112">เมื่อต้องการแก้ไขปัญหาสิทธิ์การใช้งานปฏิทินคุณสามารถใช้เครื่องมือการ[สนับสนุนและตัวช่วยการกู้คืน](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="2de44-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>