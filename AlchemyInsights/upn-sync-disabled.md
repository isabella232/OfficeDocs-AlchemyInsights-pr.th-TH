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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038131"
---
# <a name="upn-sync-disabled"></a>การซิงค์ UPN ถูกปิดใช้งาน

ถ้าคุณเริ่มซิงค์กับ Azure AD ก่อนวันที่ 30 มีนาคม 2016 ให้เรียกใช้ cmdlet PowerShell ของ Azure AD ต่อไปนี้เพื่อเปิดใช้งานการจับคู่ UPN ชั่วคราวให้กับองค์กรของคุณเท่านั้น:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -เปิดใช้งาน$True**
  
การจับคู่แบบ UPN จะเปิดใช้งานโดยอัตโนมัติในองค์กรที่เริ่มการซิงค์กับ Azure AD ในหรือหลังวันที่ 30 มีนาคม 2016
  
เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่แบบ soft บน UPN และฟีเจอร์การซิงค์อื่นๆ โปรดดู ฟีเจอร์[บริการการซิงค์ของ Azure AD เชื่อมต่อ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

