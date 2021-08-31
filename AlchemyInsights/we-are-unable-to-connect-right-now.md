---
title: ปัญหาการเปิดใช้งาน - เราไม่สามารถเชื่อมต่อได้ในขณะนี้
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744614"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>การแก้ไขMicrosoft 365 "เราไม่สามารถเชื่อมต่อได้ในขณะนี้"

หมายเหตุ: ถ้าคุณใช้งาน Windows เวอร์ชันที่เก่ากว่า (เช่น Windows 7 SP1, Windows Server 2008 R2) ให้ใช้การแก้ไขง่ายๆ เพื่อ[](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)เปิดใช้งาน TLS 1.2 เป็นค่าเริ่มต้น For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:

1. ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตMicrosoft 365แอปของคุณ ดู [URL ของ Microsoft และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP

2. ไปที่ **เริ่ม**  >  **เรียกใช้** แล้วพิมพ์ **services.msc** ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดถูกเรียกใช้อยู่:
    - การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ
    - บริการรายการเครือข่าย
    - การรับรู้สถานที่ตั้งเครือข่าย
    - Windows แฟ้มบันทึกเหตุการณ์

ถ้าหนึ่งในบริการเหล่านี้ไม่ได้เรียกใช้อยู่ ให้ลองเริ่มใช้งาน ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้การสั่งต่อไปนี้โดยการเปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล:

**sfc /scannow**

หลังจากเสร็จสิ้นการสั่งนี้ ให้รีสตาร์ตคอมพิวเตอร์

ดูข้อมูลโดยละเอียดที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง" เมื่อคุณเปิดใช้งานOfficeจากMicrosoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)