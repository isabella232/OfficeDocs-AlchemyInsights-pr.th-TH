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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233532"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>ข้อผิดพลาด 401 ไม่ได้รับอนุญาตในSharePoint

ถ้าคุณได้รับข้อผิดพลาด "(401) ไม่ได้รับอนุญาต" ใน SharePoint อาจเกี่ยวข้องกับการเลิกใช้ TLS 1.0/1.1 ดูข้อมูลเพิ่มเติมที่:

[การเตรียม 1.2 TLS ในOffice 365 Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นถ้าไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

ถ้าผู้ใช้อยู่ในWindows 7 ตรวจสอบให้แน่ใจว่า พวกเขาตรวจสอบชุดการเข้ารหัส[TLS Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)