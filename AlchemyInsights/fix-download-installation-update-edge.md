---
title: แก้ไขปัญหาเกี่ยวกับการดาวน์โหลด การติดตั้ง และการอัปเดตMicrosoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9128"
- "9004429"
ms.openlocfilehash: 3db5fc4f2be0bbf845dec15b53f1299653f97ed75e12b04e8041de5982f5a74a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812832"
---
# <a name="fix-problems-with-the-download-installation-and-update-of-microsoft-edge"></a>แก้ไขปัญหาเกี่ยวกับการดาวน์โหลด การติดตั้ง และการอัปเดตMicrosoft Edge

ก่อนที่จะพยายามแก้ไข ให้ตรวจสอบว่าระบบปฏิบัติการของคอมพิวเตอร์ของคุณเข้ากันได้กับ Microsoft Edge ซึ่งสนับสนุน Windows 10, 8, 8.1, 7 32 บิต (x86) และ 64 บิต (x64) และ macOS 10.12 Sierra และเวอร์ชันที่ใหม่กว่า เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการดาวน์โหลด Microsoft Edge และการอัปเดต ให้ปฏิบัติตามคําแนะนําเหล่านี้:

1. ตรวจสอบเครือข่ายและ VPN:
    - ตรวจสอบการเชื่อมต่อเครือข่าย
    - ข้อผิดพลาด 403 จะแนะนนะว่า VPN อาจบล็อกการดาวน์โหลดของคุณ ยกเลิกการเชื่อมต่อจาก VPN และลองMicrosoft Edgeอีกครั้ง
1. เพิ่ม officeapps.live.com ลงในรายการเว็บไซต์ที่เชื่อถือได้ของเบราว์เซอร์ของคุณ
    ตัวอย่างเช่น ถ้าคุณใช้ Internet Explorer เพื่อดาวน์โหลดMicrosoft Edge:
    1. เลือก  >  **เครื่องมือ ตัวเลือก** อินเทอร์เน็ต
    2. ใน **แท็บ** ความปลอดภัย **ให้เลือก ไซต์**  >  **ที่เชื่อถือได้**
    3. **ภายใต้ เพิ่มเว็บไซต์นี้ลงใน** โซน พิมพ์ <https://officeapps.live.com> **เลือก** เพิ่ม **แล้วเลือก** ปิด
1. ติดตั้งMicrosoft Edgeใหม่ Windowsบนคอมพิวเตอร์เครื่องหนึ่ง คุณไม่Microsoft Edgeติดตั้งอีกครั้ง นอกจากนี้ การติดตั้งใหม่จะไม่มีผลต่อประวัติ คุกกี้ และการตั้งค่าของคุณ

    บน Mac คุณต้องถอนการติดตั้งMicrosoft Edgeก่อนที่จะติดตั้งอีกครั้ง นอกจากนี้ คุณต้องคืนค่าประวัติ คุกกี้ และการตั้งค่าของคุณ

    เมื่อต้องการถอนการติดตั้งMicrosoft Edgeบน Mac:
    1. เปิด ตัวค้นหา
    2. ในโฟลเดอร์ **แอปพลิเคชัน****ให้เลือก** Microsoft Edge
    3. เลือก  >  **ไฟล์ ย้ายไปยัง** ถังขยะ

    เมื่อต้องการติดตั้งMicrosoft Edgeใหม่บนคอมพิวเตอร์ Windowsหรือ Mac:
    1. เปิดเบราว์เซอร์ใดๆ ที่ใช้งานได้
    2. ไปที่เว็บไซต์Microsoft Edgeดาวน์โหลดและติดตั้งเบราว์เซอร์อีกครั้ง
1. รีสตาร์ตคอมพิวเตอร์ของคุณ: รีสตาร์ตคอมพิวเตอร์ของคุณ และลองMicrosoft Edgeอีกครั้ง

