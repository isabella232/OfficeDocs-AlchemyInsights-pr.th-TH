---
title: การตั้งค่าหรือเปลี่ยนสิทธิ์ของโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36734688"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="ebe29-102">สิทธิ์และโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="ebe29-102">Permissions and Public Folders</span></span>

<span data-ttu-id="ebe29-103">คุณสามารถเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์สาธารณะของคุณโดยใช้ Outlook ศูนย์ดูแล Exchange (EAC), หรือ PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ebe29-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="ebe29-104">สำหรับคำแนะนำ Outlook[คลิกที่นี่](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="ebe29-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="ebe29-105">สำหรับ EAC อ้างอิงถึง[บทความนี้](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)สำหรับคำแนะนำ</span><span class="sxs-lookup"><span data-stu-id="ebe29-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="ebe29-106">สำหรับ Powershell โปรดดู[บทความนี้](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)สำหรับคำแนะนำเกี่ยวกับการใช้คำสั่ง Add-Publicfolderentญาต</span><span class="sxs-lookup"><span data-stu-id="ebe29-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="ebe29-107">ถ้าคุณต้องการคำแนะนำในการเชื่อมต่อกับ Exchange Powershell คลิกที่[นี่](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="ebe29-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="ebe29-108">ถ้า**ผู้ใช้ภายนอกไม่สามารถส่ง e-mail ไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย**เหตุผลอาจเป็นไปได้ว่าโฟลเดอร์สาธารณะไม่มีสิทธิ์ที่จำเป็นสำหรับการจัดส่งทางเมลภายนอก</span><span class="sxs-lookup"><span data-stu-id="ebe29-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="ebe29-109">คุณสามารถแก้ไขปัญหานี้โดยใช้คำแนะนำของ Outlook ที่[นี่](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)หรือคำแนะนำ PowerShell ที่[นี่](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="ebe29-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

