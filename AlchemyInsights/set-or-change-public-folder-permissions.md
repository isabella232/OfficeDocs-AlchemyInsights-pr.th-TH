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
ms.openlocfilehash: 1868b8b04df012d44781f86ee75120ca443af5be5801074329f17c0e40a5acc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060911"
---
# <a name="permissions-and-public-folders"></a>สิทธิ์และโฟลเดอร์สาธารณะ

คุณสามารถเปลี่ยนสิทธิ์ในโฟลเดอร์สาธารณะของคุณโดยใช้ Outlookศูนย์Exchange (EAC) หรือ PowerShell:
  
- เพื่อดูOutlookแนะ[นําเพิ่มเติม คลิกที่นี่](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)
    
- For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. 
    
- For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. ถ้าคุณต้องการคําแนะนําในExchange Powershell[ให้คลิก](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)ที่นี่
    
ถ้า **ผู้ใช้ภายนอกไม่สามารถส่งอีเมลไปยังโฟลเดอร์สาธารณะ** ที่เปิดใช้งานจดหมายได้ อาจเป็นเพราะโฟลเดอร์สาธารณะไม่มีสิทธิ์ที่ต้องใช้ในการส่งอีเมลภายนอก คุณสามารถแก้ไขปัญหานี้ได้โดยใช้คําแนะOutlookเหล่านี้[หรือ](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)คําแนะนําของ PowerShell[ที่นี่](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)
  

