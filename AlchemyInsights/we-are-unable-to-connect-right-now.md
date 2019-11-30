---
title: ปัญหาการเปิดใช้งาน-เราไม่สามารถเชื่อมต่อในขณะนี้
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628261"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>แก้ไขแอป Office "เราไม่สามารถเชื่อมต่อในขณะนี้" ข้อความ

ถ้าคุณได้รับข้อความนี้ให้ลองทำตามขั้นตอนต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office ดู[url ของ Office ๓๖๕และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. ไปที่**เริ่มต้น** > **รัน**และจากนั้นพิมพ์**บริการ. msc** ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดทำงานอยู่:
    - ตั้งค่าอุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้ตำแหน่งเครือข่าย
    - แฟ้มบันทึกเหตุการณ์ของ Windows

ถ้าหนึ่งในบริการเหล่านี้ไม่ได้ทำงานให้ลองเริ่มต้น ถ้าคุณมีปัญหาในการเริ่มต้นการบริการให้เรียกใช้คำสั่งต่อไปนี้โดยการเปิดพร้อมท์คำสั่งด้วยสิทธิ์ระดับสูง:

**sfc/scannow**

หลังจากคำสั่งนี้เสร็จสิ้นให้รีสตาร์ทเครื่องคอมพิวเตอร์

สำหรับข้อมูลรายละเอียดโปรดดู["ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ กรุณาลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Office ๓๖๕](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)