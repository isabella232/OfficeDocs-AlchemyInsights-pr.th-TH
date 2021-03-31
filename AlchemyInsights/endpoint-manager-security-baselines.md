---
title: ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440912"
---
# <a name="endpoint-manager---security-baselines"></a>ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย

ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยคือกลุ่มการตั้งค่า Windows ที่กําหนดค่าไว้ล่วงหน้า ซึ่งช่วยให้คุณปรับใช้การตั้งค่าความปลอดภัยที่แนะนาโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง ข้อมูลพื้นฐานเหล่านี้สามารถถูกปรับแต่งเพื่อให้แสดงเฉพาะการตั้งค่าและค่าที่ต้องการ For more information about security baselines, see [Use security baselines to configure Windows 10 devices intuns](https://docs.microsoft.com/mem/intune/protect/security-baselines).

ขณะนี้มีข้อมูลพื้นฐานเกี่ยวกับผลิตภัณฑ์เหล่านี้:

- การตั้งค่าความปลอดภัยของ Windows MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

ข้อมูลพื้นฐานแต่ละรายการจะได้รับการอัปเดตเป็นระยะๆ และเผยแพร่ในเวอร์ชันที่เพิ่มขึ้น แต่ละเวอร์ชันจะเพิ่มหรือนําการตั้งค่าออกจากเวอร์ชันก่อนหน้าเพื่อให้แน่ใจว่าข้อมูลพื้นฐานตรงตามแนวทางปัจจุบัน คอนโซลข้อมูลพื้นฐานด้านความปลอดภัยในการรักษาความปลอดภัยของจุดสิ้นสุดช่วยให้สามารถเปรียบเทียบเวอร์ชันต่างๆ ได้โดยการเปลี่ยนแปลงจากเวอร์ชันเป็นเวอร์ชันที่มองเห็นได้

สําหรับแนวทางเกี่ยวกับวิธีการเปลี่ยนอย่างมีประสิทธิภาพที่สุดว่าเวอร์ชันของแผนพื้นฐานใดได้รับการปรับใช้ ให้ดู จัดการ[โปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัยใน Microsoft Intuny](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

หลังจากการปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัย คุณสามารถตรวจสอบสถานะของการปรับใช้และการตั้งค่าการตรวจสอบบนอุปกรณ์พื้นฐาน

**หมายเหตุ:** ข้อมูลการรายงานของข้อมูลขั้นต้นอาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้ปรากฏจากการปรับใช้ครั้งแรกไปยังอุปกรณ์และสูงสุด 6 ชั่วโมงเพื่อการอัปเดตเพิ่มเติม 

สาเหตุทั่วไปของการตั้งค่าข้อมูลพื้นฐานที่ไม่ได้ใช้คือเพราะการตั้งค่าเดียวกันที่ใช้ในโปรไฟล์อื่น สถานการณ์นี้สามารถตรวจสอบอุปกรณ์ที่เฉพาะเจาะจงได้โดยการเลือกอุปกรณ์นั้นจากภายในโหนดสถานะอุปกรณ์ของโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัย For details, see [Resolve conflicts for security baselines.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)