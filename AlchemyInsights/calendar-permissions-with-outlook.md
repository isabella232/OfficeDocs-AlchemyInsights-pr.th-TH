---
title: สิทธิ์ในปฏิทิน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862165"
---
# <a name="calendar-permissions"></a><span data-ttu-id="ccf66-102">สิทธิ์ในปฏิทิน</span><span class="sxs-lookup"><span data-stu-id="ccf66-102">Calendar Permissions</span></span>

<span data-ttu-id="ccf66-103">ผู้ใช้สามารถเปลี่ยนสิทธิ์ในปฏิทินของตนเองกับ Outlook บนเว็บหรือไคลเอนต์อื่น ๆ แต่เป็นผู้ดูแลระบบคุณอาจต้องตรวจสอบเช่นกัน</span><span class="sxs-lookup"><span data-stu-id="ccf66-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="ccf66-104">ด้วย cmdlet PowerShell อัตราแลกเปลี่ยนจะแสดงสิทธิ์บนปฏิทินของผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="ccf66-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="ccf66-105">เมื่อต้องการดูข้อมูลเพิ่มเติม ให้ดูต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ccf66-105">To see more information see the following:</span></span>

- [<span data-ttu-id="ccf66-106">รับกล่องจดหมายโฟลเดอร์เปอร์mission</span><span class="sxs-lookup"><span data-stu-id="ccf66-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ccf66-107">ตั้งค่ากล่องจดหมายโฟลเดอร์เปอร์mission</span><span class="sxs-lookup"><span data-stu-id="ccf66-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ccf66-108">เพิ่มกล่องจดหมายโฟลเดอร์เปอร์mission</span><span class="sxs-lookup"><span data-stu-id="ccf66-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="ccf66-109">สิทธิ์ในปฏิทินจะใช้ในการแชร์ปฏิทิน เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการใช้ปฏิทิน Outlook ร่วมกัน ให้ดูบทความต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="ccf66-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="ccf66-110">แชร์ปฏิทิน Outlook กับบุคคลอื่น</span><span class="sxs-lookup"><span data-stu-id="ccf66-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="ccf66-111">แชร์ปฏิทินของคุณใน Outlook บนเว็บสําหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="ccf66-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="ccf66-112">เมื่อต้องการแก้ไขปัญหาสิทธิ์ในปฏิทิน คุณสามารถใช้เครื่องมือ['ตัวช่วยช่วยเหลือและการกู้คืน'](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="ccf66-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>