---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704913"
---
# <a name="troubleshoot-access-denied-messages"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ

ถ้ามีใครบางคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่แชร์ใน SharePoint ผู้ดูแลไซต์คอลเลกชันอาจเปิดใช้งาน "โหมดการจํากัดการเข้าถึงสิทธิ์การเข้าถึงของผู้ใช้" เมื่อต้องการปิดใช้งาน: 
  
1. เรียกดูไซต์ คลิกไอคอน การตั้งค่า แล้วคลิก **การตั้งค่า** ไซต์
    
2. ภายใต้ **การดูแลไซต์คอลเลกชัน** ให้คลิก **ฟีเจอร์ไซต์คอลเลกชัน**
    
3. ถัดจาก **โหมดการจํากัดสิทธิ์การเข้าถึงของผู้ใช้****ให้คลิกปิดใช้งาน**
    
ข้อความปฏิเสธการเข้าถึงสามารถเกิดขึ้นได้กับโฟลเดอร์ที่แชร์ถ้าไซต์เป็นไซต์การประกาศ For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" เมื่อพยายามดูการร้องขอการเข้าถึง ผู้ใช้จะต้องเพิ่มเป็นผู้ดูแลไซต์คอลเลกชันหรือสมาชิกของกลุ่มเจ้าของไซต์ For more info, see [Access denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).
  
ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่ถูกเอาออกจาก Active Directory ภายในองค์กรแล้วถูกเพิ่มกลับ ให้ดูการเข้าถึงถูกปฏิเสธเมื่อบัญชีผู้ใช้ถูกซิงค์กับ[Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)
  

