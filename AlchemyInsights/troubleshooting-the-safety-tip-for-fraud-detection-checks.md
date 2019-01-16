---
title: คำแนะนำด้านความปลอดภัยสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316941"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>คำแนะนำด้านความปลอดภัยสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ

ถ้าคุณกำลัง รับเคล็ดลับความปลอดภัยที่บอกว่า "ผู้ส่งล้มเหลวเช็คของเราตรวจหาการฉ้อโกง และอาจไม่สามารถที่ จะปรากฏเป็น" จาก นั้นผู้ส่งไม่สามารถผ่านการตรวจสอบการรับรองความถูกต้องเป็น DKIM หรือ SPF การแก้ปัญหานี้เป็นวิธีดีสำหรับผู้ส่งเพื่ออนุมัติด้วยตนเองได้ ถ้าผู้ส่งกำลังส่งในนามของคุณ คุณจำเป็นต้องให้สิทธิ์ดังกล่าว โดยเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ
  
ดู[คำแนะนำด้านความปลอดภัย (น่าสงสัย) สีแดงสำหรับการฉ้อโกงการตรวจหาการแก้ไขปัญหาการตรวจสอบ](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)สำหรับรายละเอียดเพิ่มเติม 
  
ต่อไปนี้เป็นบางลิงค์อื่น ๆ ที่สามารถช่วยให้:
  
- [วิธีที่ Office 365 ใช้โครงสร้างนโยบายของผู้ส่ง (SPF) เพื่อป้องกันการเคลื่อนย้าย](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [ตั้งค่า SPF ใน Office 365 เมื่อต้องการป้องกันการเคลื่อนย้าย](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

