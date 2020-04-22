---
title: การตั้งค่าหรือเปลี่ยนแปลงสิทธิ์ของโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: cf891a4db05b8a2bdb223cc86693f5072faca494
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43681123"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="b56f6-102">สิทธิ์และโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="b56f6-102">Permissions and Public Folders</span></span>

<span data-ttu-id="b56f6-103">คุณสามารถเปลี่ยนสิทธิ์บนโฟลเดอร์สาธารณะของคุณโดยใช้ Outlook ศูนย์ดูแล Exchange (EAC), หรือ PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b56f6-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="b56f6-104">สําหรับคําแนะนํา Outlook[ให้คลิก ที่นี่](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)</span><span class="sxs-lookup"><span data-stu-id="b56f6-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="b56f6-105">สําหรับ EAC โปรดดู[บทความนี้](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)สําหรับคําแนะนํา</span><span class="sxs-lookup"><span data-stu-id="b56f6-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="b56f6-106">สําหรับ Powershell อ้างอิง[ไปยังบทความนี้](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)สําหรับคําแนะนําเกี่ยวกับการใช้คําสั่งletเพิ่ม</span><span class="sxs-lookup"><span data-stu-id="b56f6-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="b56f6-107">หากคุณต้องการคําแนะนําในการเชื่อมต่อกับ Exchange Powershell ให้คลิก[ที่นี่](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="b56f6-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="b56f6-108">ถ้า**ผู้ใช้ภายนอกไม่สามารถส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย**</span><span class="sxs-lookup"><span data-stu-id="b56f6-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="b56f6-109">คุณสามารถแก้ไขปัญหานี้ได้โดยใช้คําแนะนํา Outlook[ที่นี่](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)หรือคําแนะนํา PowerShell[ที่นี่](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="b56f6-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

