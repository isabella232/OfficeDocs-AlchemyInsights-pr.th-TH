---
title: การซิงโครไนซ์โปรไฟล์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320728"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>โปรไฟล์ของฉันจะเปลี่ยนไปซิงค์กับแอปพลิเคชันโปรไฟล์SharePointเมื่อใด

SharePoint Online ใช้งานตัวจับเวลาการนําเข้า Active Directory (การนําเข้า AD) เพื่อนําเข้าผู้ใช้และกลุ่มลงในแอปพลิเคชันโปรไฟล์ผู้ใช้ 
  
1. AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลเป็นชุด
    
2. งานตัวจับเวลาจะเรียกใช้จนกว่าการเปลี่ยนแปลงจะถูกซิงค์
    
**หมายเหตุ**: ระยะเวลาที่งานต้องเรียกใช้จะขึ้นอยู่กับจํานวนการเปลี่ยนแปลงที่จะถูกประมวลผล การเปลี่ยนแปลงจํานวนมากใช้เวลานานขึ้น ข้อตกลงระดับบริการ (SLA) ระบุว่าการเปลี่ยนแปลงของผู้ใช้ในไดเรกทอรี SharePoint Online จะแสดงในแอปพลิเคชันโปรไฟล์ผู้ใช้ภายใน 24 ชั่วโมง 
  
[ข้อมูลเพิ่มเติมเกี่ยวกับการซิงค์โปรไฟล์ผู้ใช้ใน SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

