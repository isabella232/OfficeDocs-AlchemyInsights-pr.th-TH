---
title: ข้อผิดพลาดในการปิดการเชื่อมต่อที่อยู่ภายใต้SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317715"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>ข้อผิดพลาด "การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด" SharePoint

ถ้าคุณได้รับข้อผิดพลาด "การเชื่อมต่อที่ขีดเส้นใต้ถูกปิด" ใน SharePoint อาจเกี่ยวข้องกับการเลิกใช้ TLS 1.0/1.1 ดูข้อมูลเพิ่มเติมได้ที่บทความเหล่านี้:

- [การเตรียม 1.2 TLS ในOffice 365 Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นถ้าไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [อัปเดตเพื่อเปิดใช้งาน TLS 1.1 และ TLS 1.2 เป็นโพรโทคอลที่ปลอดภัยเริ่มต้นใน WinHTTP Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).