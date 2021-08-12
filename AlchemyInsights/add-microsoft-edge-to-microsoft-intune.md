---
title: เพิ่มMicrosoft EdgeไปยังMicrosoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: 19e933e3029b7b809389815026faa63ea5dc36e81c1d4eb61b52b848fa1461a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53935824"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a>เพิ่มMicrosoft EdgeไปยังMicrosoft Intune

เพื่อให้สามารถปรับใช้ กําหนดค่า ตรวจสอบ และปกป้องอุปกรณ์Microsoft Edgeการใช้งาน Windows 10 คุณจะต้องเพิ่มอุปกรณ์Microsoft Intune

> [!IMPORTANT]
- Intuned Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า
- Intuned จะตรวจหาการติดตั้งที่มีอยู่Microsoft Edgeโดยอัตโนมัติ
- ถ้าคุณMicrosoft Edgeในบริบทของผู้ใช้ การติดตั้งระบบจะเขียนทับการติดตั้งในบริบทของผู้ใช้
- ถ้าคุณMicrosoft Edgeในบริบทของระบบ ความสาเร็จในการติดตั้งจะได้รับรายงาน
- Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.

**เบื้องต้น**

Windows 10เวอร์ชัน 1709 หรือใหม่กว่า

**ขั้นตอนในการเพิ่ม Microsoft Edge ลงใน Intuned**

1. [กําหนดค่าแอปใน Intun1](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
2. [กําหนดค่าข้อมูล](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป
3. [กําหนดค่าการตั้งค่า](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป
4. [เลือกแท็กขอบเขต (ไม่บังคับ)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
5. [เพิ่ม](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป

หากต้องการความช่วยเหลือเพิ่มเติม [โปรดดูที่](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)การแก้ไขปัญหา




