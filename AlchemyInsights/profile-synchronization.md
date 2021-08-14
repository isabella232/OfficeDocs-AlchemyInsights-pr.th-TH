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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923663"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>โปรไฟล์ของฉันจะซิงค์กับแอปพลิเคชันโปรไฟล์SharePointโปรไฟล์ผู้ใช้เมื่อใด

SharePoint Online ใช้งานตัวจับเวลาการนําเข้า Active Directory (การนําเข้า AD) เพื่อนําเข้าผู้ใช้และกลุ่มลงในแอปพลิเคชันโปรไฟล์ผู้ใช้ 
  
1. AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. การเปลี่ยนแปลงเหล่านี้จะถูกประมวลผลเป็นชุด
    
2. งานตัวจับเวลาจะเรียกใช้จนกว่าการเปลี่ยนแปลงจะถูกซิงค์
    
> [!NOTE]
> เวลาที่งานจะเรียกใช้จะขึ้นอยู่กับจํานวนการเปลี่ยนแปลงที่จะถูกประมวลผล การเปลี่ยนแปลงจํานวนมากใช้เวลานานขึ้น ข้อตกลงระดับบริการ (SLA) ระบุว่าการเปลี่ยนแปลงของผู้ใช้ในไดเรกทอรี SharePoint Online จะแสดงในแอปพลิเคชันโปรไฟล์ผู้ใช้ภายใน 24 ชั่วโมง 
  
[ข้อมูลเพิ่มเติมเกี่ยวกับการซิงค์โปรไฟล์ผู้ใช้ใน SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

