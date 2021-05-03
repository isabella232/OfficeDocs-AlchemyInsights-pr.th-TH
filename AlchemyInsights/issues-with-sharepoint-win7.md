---
title: ปัญหาเกี่ยวกับSharePointบนเครื่อง Windows 7 เครื่อง
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125520"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>ปัญหาเกี่ยวกับSharePointบนเครื่อง Windows 7 เครื่อง

ถ้าคุณได้รับข้อผิดพลาดบน Windows 7 เครื่องขณะSharePoint OneDrive หรือ OneDrive เครื่องอาจเกี่ยวข้องกับการเลิกใช้ TLS 1.0/1.1 สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [การเตรียม 1.2 TLS ในOffice 365 Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windowsไคลเอ็นต์ 7 SP1/Windows 8ต้องมีการเปิดใช้งาน TLS1.2 For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- ติดตั้ง KB3140245 และสร้างค่ารีจิสทรี For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windowsไคลเอ็นต์ 7 SP1/Windows 8 ต้องตรวจสอบให้แน่ใจว่าชุดการเข้ารหัส TLS ล่าสุดได้รับการติดตั้งแล้ว ดูข้อมูลเพิ่มเติมที่ ที่ปรึกษา[ด้านความปลอดภัยของ Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


