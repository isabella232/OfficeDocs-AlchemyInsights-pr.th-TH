---
title: การซิงค์ UPN ถูกปิดใช้งาน
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782170"
---
# <a name="upn-sync-disabled"></a>การซิงค์ UPN ถูกปิดใช้งาน

ถ้าคุณเริ่มซิงค์กับ Azure AD ก่อนวันที่ 30 มีนาคม 2016 ให้เรียกใช้ cmdlet PowerShell ของ Azure AD ต่อไปนี้เพื่อเปิดใช้งานการจับคู่ UPN ชั่วคราวให้กับองค์กรของคุณเท่านั้น:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -เปิดใช้งาน$True**
  
การจับคู่แบบ UPN จะเปิดใช้งานโดยอัตโนมัติในองค์กรที่เริ่มการซิงค์กับ Azure AD ในหรือหลังวันที่ 30 มีนาคม 2016
  
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่แบบ Soft บน UPN และฟีเจอร์การซิงค์อื่นๆ โปรดดู ฟีเจอร์บริการ[การซิงค์ Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

