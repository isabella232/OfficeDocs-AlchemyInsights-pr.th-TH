---
title: การแก้ไขแอป Office Sorry เรากําลังมีข้อความเกี่ยวกับปัญหาเซิร์ฟเวอร์ชั่วคราว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764136"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>การแก้ไขแอป Office "ขออภัย เรากําลังมีปัญหาชั่วคราวของเซิร์ฟเวอร์"

ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**เริ่ม** > **เรียกใช้**แล้วพิมพ์**services.msc** ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้กําลังทํางานอยู่ทั้งหมด:
    - อุปกรณ์ที่เชื่อมต่อเครือข่ายอัตโนมัติติดตั้ง
    - บริการรายการเครือข่าย
    - การรับรู้ตําแหน่งบนเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

ถ้าบริการเหล่านี้ไม่ได้ทํางานอยู่ ให้ลองเริ่มการทํางาน ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้โดยการเปิดพร้อมท์คําสั่งที่มีสิทธิ์ผู้ดูแล:

**sfc /สแกนโนว**

หลังจากคําสั่งนี้เสร็จสิ้น ให้รีสตาร์ทคอมพิวเตอร์

สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"ข้อผิดพลาดเมื่อคุณเปิดใช้งาน](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)