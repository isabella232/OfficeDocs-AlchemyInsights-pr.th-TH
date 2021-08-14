---
title: การตั้งค่านโยบายการป้องกันแอป Android ใน Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: ff253ad4b2ba12e25a786b5aa5bac76ae4765206a2e12880a0673ce5fcbf30c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951656"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a>การตั้งค่านโยบายการป้องกันแอป Android ใน Microsoft Intune

การตั้งค่านโยบายการป้องกันแอปบนอุปกรณ์ Android มีอยู่สามประเภท:

**การป้องกัน** ข้อมูล จะควบคุมวิธีการจัดการข้อมูลบริษัท เช่น ไม่ว่าจะเป็นการคัดลอกและวางข้อมูลลงในแอปอื่น หรือจะถ่ายสกรีนช็อตของแอปหรือไม่ นอกจากนี้ การตั้งค่ายังบังคับใช้การเข้ารหัสลับกับข้อมูลของบริษัทและจัดการว่าสามารถซิงค์ข้อมูลบางอย่างกับแอปของอุปกรณ์ดั้งเดิม เช่น รายการที่ติดต่อหรือเว็บเบราว์เซอร์ได้ เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู การป้องกัน](https://go.microsoft.com/fwlink/?linkid=2135259)ข้อมูล

**ข้อแ** นะนาของ Access จะแนะแนววิธีที่ผู้ใช้สามารถเข้าถึงแอป For example, an app could require the user to enter a PIN or fingerprint to access it. เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [ความต้องการของ](https://go.microsoft.com/fwlink/?linkid=2135260)Access

**การเปิดใช้งาน** ตามเงื่อนไขจะควบคุมการตั้งค่าความปลอดภัยในการลงชื่อเข้าใช้ของแอป เช่น ความพยายามในการกด PIN สูงสุดก่อนการล็อกหรือระบบปฏิบัติการขั้นต่าที่ต้องใช้ในการเรียกใช้แอป เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [เปิดใช้](https://go.microsoft.com/fwlink/?linkid=2135507)ตามเงื่อนไข
