---
title: สร้างกลุ่ม
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
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929324"
---
# <a name="create-a-group"></a>สร้างกลุ่ม

หัวข้อนี้จะอธิบายเกี่ยวกับการสร้างกลุ่ม

**สิทธิ์ในการสร้างกลุ่ม**

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่ ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัล Azure หรือแผงการเข้าถึงได้ คุณอาจต้องใช้ผู้ดูแลระบบเพื่อสร้างกลุ่มใหม่ให้คุณ หรือมอบสิทธิ์ที่เหมาะสมแก่คุณ

**จัดการสิทธิ์การสร้างกลุ่ม**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การสร้างกลุ่ม (ด้วยเหตุผลด้านความปลอดภัย) หรือกลุ่ม Office 365 ที่สร้างขึ้นในพอร์ทัล Azure หรือแผงการเข้าถึง โดยการเลือก "ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล Azure" หรือ "ผู้ใช้สามารถสร้างกลุ่ม Office 365 ในพอร์ทัล Azure" ในตัวเลือกกลุ่มทั้งหมด ทั่วไป  >  **(การตั้งค่า)**
2. You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.

**การปิดใช้งานการแจ้งเตือนต้อนรับของสมาชิกOffice 365ใหม่**

การแจ้งเตือนต้อนรับที่ส่งไปยังผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office 365 อาจถูกปิดใช้งานโดยการตั้งค่า **UnifiedGroupWelcomedMessageEnabled** เป็น เท็จ ใน Powershell เรียนรู้เกี่ยวกับการตั้งค่า [นี้](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)ที่นี่

