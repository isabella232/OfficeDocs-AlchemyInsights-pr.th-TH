---
title: ปัญหาการเปิดใช้งาน - เราไม่สามารถเชื่อมต่อได้ในขณะนี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716191"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>การแก้ไขแอป Office "เราไม่สามารถเชื่อมต่อได้ในขณะนี้"

ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office ดู[URL ของ Microsoft และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**เริ่ม** > **เรียกใช้**แล้วพิมพ์**services.msc** ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้กําลังทํางานอยู่ทั้งหมด:
    - อุปกรณ์ที่เชื่อมต่อเครือข่ายอัตโนมัติติดตั้ง
    - บริการรายการเครือข่าย
    - การรับรู้ตําแหน่งบนเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

ถ้าบริการเหล่านี้ไม่ได้ทํางานอยู่ ให้ลองเริ่มการทํางาน ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้โดยการเปิดพร้อมท์คําสั่งที่มีสิทธิ์ผู้ดูแล:

**sfc /สแกนโนว**

หลังจากคําสั่งนี้เสร็จสิ้น ให้รีสตาร์ทคอมพิวเตอร์

สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)