---
title: การแก้ไขปัญหาด้านความปลอดภัยสำหรับการตรวจสอบการตรวจสอบการฉ้อโกง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658429"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>การแก้ไขปัญหาด้านความปลอดภัยสำหรับการตรวจสอบการตรวจสอบการฉ้อโกง

ถ้าคุณได้รับคำแนะนำด้านความปลอดภัยที่ระบุว่า "ผู้ส่งไม่สามารถตรวจสอบการฉ้อโกงของเราได้และอาจไม่ใช่บุคคลที่พวกเขาปรากฏเป็น" จากนั้นผู้ส่งไม่สามารถส่งผ่าน DKIM หรือตรวจสอบการรับรองความถูกต้องของ SPF ได้ วิธีที่ดีที่สุดในการแก้ไขปัญหานี้มีไว้สำหรับผู้ส่งเพื่ออนุญาตตัวเอง ถ้าผู้ส่งถูกส่งในนามของคุณคุณจำเป็นต้องได้รับอนุญาตโดยการเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ
  
ให้ดู [ที่การแก้ไขปัญหาด้านความปลอดภัยของสีแดง (ที่น่าสงสัย) สำหรับการตรวจสอบการตรวจสอบการฉ้อโกง](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) สำหรับข้อมูลเพิ่มเติม
  
ต่อไปนี้เป็นลิงก์อื่นๆที่สามารถช่วยได้:
  
- [วิธีที่ Microsoft ใช้กรอบนโยบายผู้ส่ง (SPF) เพื่อป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [ตั้งค่า SPF เพื่อช่วยป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
