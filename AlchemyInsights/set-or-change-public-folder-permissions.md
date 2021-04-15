---
title: ตั้งค่าหรือเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789226"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="02b8b-102">สิทธิ์และโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="02b8b-102">Permissions and Public Folders</span></span>

<span data-ttu-id="02b8b-103">คุณสามารถเปลี่ยนสิทธิ์ในโฟลเดอร์สาธารณะของคุณโดยใช้ Outlook, Exchange admin center (EAC) หรือ PowerShell:</span><span class="sxs-lookup"><span data-stu-id="02b8b-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="02b8b-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="02b8b-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="02b8b-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span><span class="sxs-lookup"><span data-stu-id="02b8b-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="02b8b-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="02b8b-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="02b8b-107">ถ้าคุณต้องการคําแนะนําในการเชื่อมต่อกับ Exchange Powershell [ให้คลิก](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)ที่นี่</span><span class="sxs-lookup"><span data-stu-id="02b8b-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="02b8b-108">ถ้า **ผู้ใช้ภายนอกไม่สามารถส่งอีเมลไปยังโฟลเดอร์สาธารณะ** ที่เปิดใช้งานจดหมายได้ อาจเป็นเพราะโฟลเดอร์สาธารณะไม่มีสิทธิ์ที่ต้องใช้ในการส่งอีเมลภายนอก</span><span class="sxs-lookup"><span data-stu-id="02b8b-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="02b8b-109">คุณสามารถแก้ไขปัญหานี้ได้โดยใช้คําแนะนําของ Outlook[ที่นี่](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)หรือคําแนะนําของ PowerShell[ที่นี่](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="02b8b-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

