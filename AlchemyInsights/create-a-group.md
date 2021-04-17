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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816391"
---
# <a name="create-a-group"></a>สร้างกลุ่ม

หัวข้อนี้จะอธิบายเกี่ยวกับการสร้างกลุ่ม

**สิทธิ์ในการสร้างกลุ่ม**

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่ ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัล Azure หรือแผงการเข้าถึงได้ คุณอาจต้องใช้ผู้ดูแลระบบเพื่อสร้างกลุ่มใหม่ให้คุณ หรือมอบสิทธิ์ที่เหมาะสมแก่คุณ

**จัดการสิทธิ์การสร้างกลุ่ม**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การสร้างกลุ่ม (ด้วยเหตุผลด้านความปลอดภัย) หรือกลุ่ม Office 365 ที่สร้างขึ้นในพอร์ทัล Azure หรือแผงการเข้าถึง โดยเลือก "ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล Azure" หรือ "ผู้ใช้สามารถสร้างกลุ่ม Office 365 ในพอร์ทัลAzure" ใน ตัวเลือก กลุ่มทั้งหมด  >  **ทั่วไป (การตั้งค่า)**
2. คุณยังสามารถจํากัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ ถ้าคุณมีสิทธิ์การใช้งาน Azure Active Directory P1 Premium

**การปิดใช้งานการแจ้งเตือนต้อนรับของสมาชิกกลุ่ม Office 365 ใหม่**

การแจ้งเตือนต้อนรับที่ส่งถึงผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office 365 สามารถถูกปิดใช้งานโดยการตั้งค่า **UnifiedGroupWelcomesMessageEnabled** เป็น False ใน Powershell เรียนรู้เกี่ยวกับการตั้งค่า [นี้](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)ที่นี่

