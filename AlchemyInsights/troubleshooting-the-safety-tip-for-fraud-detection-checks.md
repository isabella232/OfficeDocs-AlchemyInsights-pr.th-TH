---
title: การแก้ไขปัญหาเกี่ยวกับคําเตือนด้านความปลอดภัยตรวจหาการฉ้อฉล
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955985"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>การแก้ไขปัญหาเกี่ยวกับคําเตือนด้านความปลอดภัยตรวจหาการฉ้อฉล

ถ้าคุณได้รับเอกสาร คําเตือนด้านความปลอดภัย ที่ระบุว่า "ผู้ส่งล้มเหลวในการตรวจหาการหลอกลวงของเราและอาจไม่ใช่บุคคลที่พวกเขาปรากฏ" ผู้ส่งล้มเหลวในการผ่านการตรวจสอบการรับรองความถูกต้อง DKIM หรือ SPF วิธีที่ดีที่สุดในการแก้ไขปัญหานี้คือให้ผู้ส่งอนุมัติตนเอง ถ้าผู้ส่งส่งในนามของคุณ คุณต้องอนุญาตโดยการเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ
  
ดู[การแก้ไขปัญหาเครือข่ายสีแดง (น่าสงสัย) คําเตือนด้านความปลอดภัยตรวจหาการฉ้อ](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)ฉล ตรวจหาข้อมูลเพิ่มเติม
  
ต่อไปนี้คือลิงก์อื่นๆ บางส่วนที่สามารถช่วยได้:
  
- [วิธีการที่ Microsoft ใช้เฟรมเวิร์กนโยบายผู้ส่ง (SPF) เพื่อป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [ตั้งค่า SPF เพื่อช่วยป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
