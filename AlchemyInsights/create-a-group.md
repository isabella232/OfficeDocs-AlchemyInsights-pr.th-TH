---
title: สร้างกลุ่ม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089178"
---
# <a name="create-a-group"></a>สร้างกลุ่ม

หัวข้อนี้จะอธิบายเกี่ยวกับการสร้างกลุ่ม

**สิทธิ์ในการสร้างกลุ่ม**

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่ ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัลไซต์ Azure หรือแผงการเข้าถึง คุณอาจจำเป็นต้องมีผู้ดูแลระบบในการสร้างกลุ่มใหม่ให้กับคุณหรือเพื่อให้สิทธิ์ที่เหมาะสมกับคุณ

**จัดการสิทธิ์ในการสร้างกลุ่ม**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์ในการสร้างกลุ่มได้ (สำหรับเหตุผลด้านความปลอดภัย) หรือกลุ่ม Office ๓๖๕ที่สร้างขึ้นในพอร์ทัล azure หรือแผงการเข้าถึงโดยการเลือก "ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล azure" หรือ "ผู้ใช้สามารถสร้างกลุ่ม Office ๓๖๕ในพอร์ทัลไซต์ azure" ได้ในตัวเลือกใน **กลุ่ม**  >  **ทั่วไป (การตั้งค่า)**
2. นอกจากนี้คุณยังสามารถจำกัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ถ้าคุณมีสิทธิ์การใช้งาน Azure ของไดเรกทอรีที่ใช้งานอยู่ของ Azure

**การปิดใช้งานการแจ้งให้ทราบยินดีต้อนรับสำหรับสมาชิกกลุ่ม Office ๓๖๕ใหม่**

การแจ้งเตือนยินดีต้อนรับที่ส่งไปยังผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office ๓๖๕สามารถปิดใช้งานได้โดยการตั้งค่า **UnifiedGroupWelcomeMessageEnabled** เป็น False ใน Powershell เรียนรู้เกี่ยวกับการตั้งค่านี้[ที่นี่](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

