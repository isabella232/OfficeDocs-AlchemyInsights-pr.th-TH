---
title: ซิงค์ UPN ที่ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493478"
---
# <a name="upn-sync-disabled"></a>ซิงค์ UPN ที่ถูกปิดใช้งาน

ถ้าคุณเริ่มต้นทำการซิงค์กับโฆษณา Azure ก่อน 30 มีนาคม 2016 เรียกใช้ cmdlet PowerShell โฆษณา Azure ต่อไปนี้เพื่อเปิดใช้งานการจับคู่นุ่ม UPN สำหรับองค์กรของคุณเท่านั้น:
  
 **ชุด MsolDirSyncFeature-คุณลักษณะ EnableSoftMatchOnUpn-$True การเปิดใช้งาน**
  
จับคู่นุ่ม UPN จะเปิดโดยอัตโนมัติสำหรับองค์กรที่เริ่มซิงค์ Azure โฆษณาใน หรือหลัง จากวันที่ 30 มีนาคม 2016
  
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่นุ่ม UPN และคุณลักษณะการซิงค์อื่น ๆ โปรดดู[ลักษณะการทำงานการบริการซิงค์เชื่อมต่อ AD Azure](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

