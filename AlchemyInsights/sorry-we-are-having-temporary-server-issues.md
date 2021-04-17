---
title: การแก้ไขแอป Microsoft 365 ขออภัย เราอยู่ในข้อความปัญหาของเซิร์ฟเวอร์ชั่วคราว
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835290"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>การแก้ไขข้อความ "ขออภัย เราพบปัญหาเซิร์ฟเวอร์ชั่วคราว" ของแอป Microsoft 365

ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365 ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP

2. ไปที่ **เริ่ม**  >  **เรียกใช้** แล้วพิมพ์ **services.msc** ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดถูกเรียกใช้อยู่:
    - การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้สถานที่ตั้งเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

ถ้าหนึ่งในบริการเหล่านี้ไม่ได้เรียกใช้อยู่ ให้ลองเริ่มใช้งาน ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้สั่งต่อไปนี้โดยการเปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล:

**sfc /scannow**

หลังจากเสร็จสิ้นการสั่งนี้ ให้รีสตาร์ตคอมพิวเตอร์

ดูข้อมูลโดยละเอียดที่ ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ ข้อผิดพลาด โปรดลองอีกครั้งในภายหลัง" เมื่อคุณ](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)เปิดใช้งาน