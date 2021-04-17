---
title: การแก้ไขปัญหาเคล็ดลับความปลอดภัยเพื่อตรวจสอบการตรวจหาการหลอกลวง
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834750"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>การแก้ไขปัญหาเคล็ดลับความปลอดภัยเพื่อตรวจสอบการตรวจหาการหลอกลวง

ถ้าคุณได้รับเคล็ดลับความปลอดภัยที่ระบุว่า "ผู้ส่งล้มเหลวในการตรวจสอบการหลอกลวงของเราและอาจไม่ใช่บุคคลที่พวกเขาปรากฏ" ผู้ส่งล้มเหลวในการผ่านการตรวจสอบการรับรองความถูกต้อง DKIM หรือ SPF วิธีที่ดีที่สุดในการแก้ไขปัญหานี้คือให้ผู้ส่งอนุมัติตนเอง ถ้าผู้ส่งส่งในนามของคุณ คุณต้องอนุญาตโดยการเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ
  
ดู [การแก้ไขปัญหาเคล็ดลับความปลอดภัยสีแดง (น่าสงสัย) เพื่อตรวจสอบการตรวจสอบการหลอกลวง](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) เพื่อดูข้อมูลเพิ่มเติม
  
ต่อไปนี้คือลิงก์อื่นๆ บางส่วนที่สามารถช่วยได้:
  
- [วิธีการที่ Microsoft ใช้เฟรมเวิร์กนโยบายผู้ส่ง (SPF) เพื่อป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [ตั้งค่า SPF เพื่อช่วยป้องกันการปลอมแปลง](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
