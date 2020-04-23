---
title: การแก้ไขปัญหาเกี่ยวกับเคล็ดลับความปลอดภัยสําหรับการตรวจสอบการทุจริต
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759531"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>การแก้ไขปัญหาเกี่ยวกับเคล็ดลับความปลอดภัยสําหรับการตรวจสอบการทุจริต

หากคุณได้รับคําแนะนําด้านความปลอดภัยที่ระบุว่า "ผู้ส่งตรวจสอบการฉ้อโกงของเราล้มเหลว และอาจไม่ใช่ผู้ส่งที่ถูกส่งผ่านการตรวจสอบสิทธิ์ DKIM หรือ SPF วิธีที่ดีที่สุดในการแก้ไขปัญหานี้คือเพื่อให้ผู้ส่งอนุญาตด้วยตนเอง หากผู้ส่งส่งในนามของคุณ คุณจําเป็นต้องอนุญาตผู้ส่งโดยการเพิ่มที่อยู่ IP ของผู้ส่งลงในระเบียน SPF ของคุณ
  
โปรดดู[ข้อมูลเพิ่มเติมใน การแก้ไขปัญหาเคล็ดลับความปลอดภัยสีแดง (ที่น่าสงสัย) สําหรับการตรวจสอบการตรวจหาการฉ้อโกง](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
ต่อไปนี้เป็นลิงก์อื่น ๆ ที่สามารถช่วย:
  
- [วิธีการที่ Microsoft ใช้กรอบการทํางานของนโยบายผู้ส่ง (SPF) เพื่อป้องกันการปลอมแปลง](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [ตั้งค่า SPF เพื่อช่วยป้องกันการปลอมแปลง](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
