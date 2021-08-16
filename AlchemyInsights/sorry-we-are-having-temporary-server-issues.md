---
title: การแก้ไขMicrosoft 365แอปต่างๆ ขออภัย เราได้รับข้อความแสดงปัญหาของเซิร์ฟเวอร์ชั่วคราว
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021615"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>การแก้ไขปัญหาMicrosoft 365 "ขออภัย เราพบปัญหาเซิร์ฟเวอร์ชั่วคราว"

ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:

1. ตรวจสอบการตั้งค่าไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตMicrosoft 365แอปของคุณ ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP

2. ไปที่ **เริ่ม**  >  **เรียกใช้** แล้วพิมพ์ **services.msc** ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดถูกเรียกใช้อยู่:
    - การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้สถานที่ตั้งเครือข่าย
    - Windows แฟ้มบันทึกเหตุการณ์

ถ้าหนึ่งในบริการเหล่านี้ไม่ได้เรียกใช้อยู่ ให้ลองเริ่มใช้งาน ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้สั่งต่อไปนี้โดยการเปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล:

**sfc /scannow**

หลังจากเสร็จสิ้นการสั่งนี้ ให้รีสตาร์ตคอมพิวเตอร์

ดูข้อมูลโดยละเอียดที่ ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ ข้อผิดพลาด โปรดลองอีกครั้งในภายหลัง" เมื่อคุณ](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)เปิดใช้งาน