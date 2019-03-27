---
title: ตั้งค่า หรือเปลี่ยนแปลงสิทธิ์ของโฟลเดอร์สาธารณะ
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
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767303"
---
# <a name="permissions-and-public-folders"></a>การอนุญาตและโฟลเดอร์สาธารณะ

คุณสามารถเปลี่ยนแปลงสิทธิ์บนโฟลเดอร์สาธารณะของคุณโดยใช้ Outlook ศูนย์กลางการดูแล Exchange (EAC), หรือ PowerShell:
  
- สำหรับ Outlook คำแนะนำ[คลิกที่นี่](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)
    
- สำหรับ EAC อ้างอิงถึง[บทความนี้](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)สำหรับคำแนะนำ คุณสามารถคลิ[ที่นี่](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx)เพื่อไปยัง EAC ได้ 
    
- สำหรับ Powershell อ้างอิงถึง[บทความนี้](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)สำหรับคำแนะนำเกี่ยวกับการเพิ่ม PublicFolderClientPermission commandlet ใช้ ถ้าคุณต้องการให้คำแนะนำเพื่อเชื่อมต่อกับ Exchange Powershell คลิก[ที่นี่](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)
    
ถ้า**ผู้ใช้ภายนอกไม่สามารถส่งอีเมล์ไปยังจดหมายเปิดใช้งานโฟลเดอร์สาธารณะ**เหตุผลอาจ โฟลเดอร์สาธารณะไม่มีสิทธิ์ที่จำเป็นสำหรับการส่งอีเมภายนอก คุณสามารถแก้ไขปัญหานี้โดยใช้คำแนะนำของ Outlook[ที่นี่](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)หรือคำสั่ง PowerShell[ที่นี่](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)ได้
  

