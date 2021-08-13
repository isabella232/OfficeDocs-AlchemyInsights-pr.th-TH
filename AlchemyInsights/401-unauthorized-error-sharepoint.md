---
title: ข้อผิดพลาด 401 ไม่ได้รับอนุญาตในSharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919046"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>ข้อผิดพลาด 401 ไม่ได้รับอนุญาตในSharePoint

ถ้าคุณได้รับข้อผิดพลาด "(401) ไม่ได้รับอนุญาต" ใน SharePoint อาจเกี่ยวข้องกับการเลิกใช้ TLS 1.0/1.1 ดูข้อมูลเพิ่มเติมที่:

- [การเตรียม 1.2 TLS ในOffice 365 Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นถ้าไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [อัปเดตเพื่อเปิดใช้งาน TLS 1.1 และ TLS 1.2 เป็นโพรโทคอลที่ปลอดภัยเริ่มต้นใน WinHTTP Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

ถ้าผู้ใช้อยู่ในWindows 7 ตรวจสอบให้แน่ใจว่า พวกเขาตรวจสอบชุดการเข้ารหัส[TLS Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)