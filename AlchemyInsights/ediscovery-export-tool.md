---
title: เครื่องมือส่งออก eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101321"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>ไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery ได้ใช่ไหม

ถ้าคุณไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery เพื่อดาวน์โหลดผลลัพธ์การค้นหา ให้ตรวจสอบสิ่งต่อไปนี้:
  
- คอมพิวเตอร์ที่คุณใช้งานตรงตามเงื่อนไขต่อไปนี้:

  - เวอร์ชัน 32 บิตหรือ 64 บิตWindows 7 และเวอร์ชันที่ใหม่กว่า

  - Microsoft .NET Framework 4.7

  - เบราว์เซอร์ที่สนับสนุน:

  - Microsoft Edge

    หรือ

  - Internet Explorer 10และเวอร์ชันที่ใหม่กว่า

    เบราว์เซอร์อื่นๆ เช่น Google Chrome และ Mozilla Firefox ไม่ได้รับการสนับสนุน

- องค์กรของคุณสามารถเชื่อมต่อกับจุดสิ้นสุดใน Azure ซึ่งเป็น **\* .blob.core.windows.net** (อักขระตัวแทนจะแสดงตัวระบุเฉพาะของงานส่งออกของคุณ)

- คุณได้รับมอบหมายบทบาทส่งออกในศูนย์การปฏิบัติตามMicrosoft 365 &amp; การรักษาความปลอดภัยของไมโครซอฟท์ ตามค่าเริ่มต้น บทบาทนี้จะถูกมอบหมายให้กับกลุ่มบทบาทตัวจัดการ eDiscovery เท่านั้น ดู[กําหนดสิทธิ์ eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก: การส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า[100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)