---
title: การแก้ไขปัญหาการเข้าถึงข้อความถูกปฏิเสธ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939902"
---
# <a name="troubleshoot-access-denied-messages"></a>การแก้ไขปัญหาการเข้าถึงข้อความถูกปฏิเสธ

ถ้ามีใครบางคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" ไปยังโฟลเดอร์ที่แชร์ใน SharePoint ผู้ดูแลไซต์คอลเลกชันอาจเปิดใช้งาน "โหมดการจํากัดการเข้าถึงสิทธิ์ผู้ใช้" เมื่อต้องการปิดใช้งาน: 
  
1. เรียกดูไซต์ คลิกการตั้งค่าไซต์ จากนั้นคลิก ตัวเลือก **การตั้งค่า**
    
2. ภายใต้ **การดูแลไซต์คอลเลกชัน** ให้คลิก **ฟีเจอร์ของ** ไซต์คอลเลกชัน
    
3. ถัดจาก **โหมดการจํากัดสิทธิ์การเข้าถึงของผู้ใช้** ให้คลิก **ปิดใช้งาน**
    
ข้อความปฏิเสธการเข้าถึงยังสามารถเกิดขึ้นได้กับโฟลเดอร์ที่แชร์ถ้าไซต์เป็นไซต์การประกาศ ดูข้อมูลเพิ่มเติมได้ที่ [การเข้าถึงถูกปฏิเสธเมื่อเข้าถึงโฟลเดอร์ที่](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)แชร์
  
ถ้าใครบางคนได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" เมื่อพยายามดูการร้องขอการเข้าถึง ผู้ใช้จะต้องถูกเพิ่มเป็นผู้ดูแลไซต์คอลเลกชันหรือสมาชิกของกลุ่มเจ้าของไซต์ For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).
  
ถ้าผู้ใช้ได้รับข้อความ "การเข้าถึงถูกปฏิเสธ" หลังจากที่ถูกเอาออกจาก Active Directory ภายในองค์กร แล้วเพิ่มกลับ ให้ดู การเข้าถึงถูกปฏิเสธ[](https://go.microsoft.com/fwlink/?linkid=2004318)เมื่อบัญชีผู้ใช้ถูกซิงค์Microsoft 365
  

