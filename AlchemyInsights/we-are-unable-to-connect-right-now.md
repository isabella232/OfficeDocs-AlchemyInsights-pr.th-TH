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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581894"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>การแก้ไขแอป Microsoft 365 "เราไม่สามารถเชื่อมต่อได้ในขณะนี้" ข้อความ

หากคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365 ดู[URL ของ Microsoft และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**Start**  >  **เริ่มรัน**แล้วพิมพ์**services.msc** ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้ทั้งหมดทํางาน:
    - อุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้ตําแหน่งบนเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

หากบริการใดบริการหนึ่งเหล่านี้ไม่ทํางาน ให้ลองเริ่มต้นบริการดังกล่าว ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้ โดยการเปิดพร้อมท์คําสั่งด้วยสิทธิ์ผู้ดูแล:

**/ สแกน**

หลังจากคําสั่งนี้เสร็จสิ้น แล้ว ให้รีสตาร์ทคอมพิวเตอร์

สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)