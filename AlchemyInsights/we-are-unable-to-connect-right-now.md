---
title: ปัญหาการเปิดใช้งาน-เราไม่สามารถเชื่อมต่อได้ในขณะนี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726002"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>การแก้ไขแอป Microsoft ๓๖๕ "เราไม่สามารถเชื่อมต่อได้ในขณะนี้" ข้อความ

ถ้าคุณได้รับข้อความนี้ให้ลองทำดังต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft ๓๖๕ ให้ดู[ที่ url และช่วงที่อยู่ IP ของ Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**เริ่ม**  >  **เรียกใช้**แล้วพิมพ์**msc** ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้กำลังทำงานอยู่ทั้งหมด:
    - การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้ตำแหน่งบนเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

ถ้าหนึ่งในบริการเหล่านี้ไม่ได้ทำงานอยู่ให้ลองเริ่มต้นใช้งาน ถ้าคุณมีปัญหาในการเริ่มบริการให้เรียกใช้คำสั่งต่อไปนี้โดยการเปิดพร้อมท์คำสั่งด้วยสิทธิ์ผู้ดูแล:

**sfc/scannow**

หลังจากคำสั่งนี้เสร็จสิ้นให้รีสตาร์ตเครื่องคอมพิวเตอร์

สำหรับข้อมูลโดยละเอียดให้ดู[ที่ "ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีผู้ใช้ของคุณได้ โปรดลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Microsoft ๓๖๕](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)