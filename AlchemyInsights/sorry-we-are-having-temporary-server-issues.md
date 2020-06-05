---
title: การแก้ไขแอป Microsoft 365 ขออภัยเรากําลังมีปัญหาเซิร์ฟเวอร์ชั่วคราว
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582722"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>การแก้ไขแอป Microsoft 365 "ขออภัยเรากําลังมีปัญหาเซิร์ฟเวอร์ชั่วคราว"

หากคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365 ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**Start**  >  **เริ่มรัน**แล้วพิมพ์**services.msc** ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้ทั้งหมดทํางาน:
    - อุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้ตําแหน่งบนเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

หากบริการใดบริการหนึ่งเหล่านี้ไม่ทํางาน ให้ลองเริ่มต้นบริการดังกล่าว ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้ โดยการเปิดพร้อมท์คําสั่งด้วยสิทธิ์ผู้ดูแล:

**/ สแกน**

หลังจากคําสั่งนี้เสร็จสิ้น แล้ว ให้รีสตาร์ทคอมพิวเตอร์

สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)