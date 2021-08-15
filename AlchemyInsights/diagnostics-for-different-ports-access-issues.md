---
title: การวินิจฉัยปัญหาการเข้าถึงพอร์ตต่างๆ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030921"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>การวินิจฉัยปัญหาการเข้าถึงพอร์ตต่างๆ

เมื่อต้องการแก้ไขปัญหาการเข้าถึงพอร์ตต่างๆ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. หยุด/จัดการเครื่องเสมือน (VM) จากพอร์ทัล เริ่ม VM ใหม่ แล้วทดสอบอีกครั้ง 
2. ตรวจสอบการตั้งค่าเครือข่ายของ VM ของคุณเพื่อตรวจสอบว่าคุณมีกลุ่มความปลอดภัยของเครือข่าย (NSGs) บล็อกการรับส่งข้อมูลหรือไม่ คุณยังสามารถใช้เครื่องมือตรวจสอบเส้นทาง IP ของ [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) เพื่อตรวจสอบ NSGs ที่บล็อกการรับส่งข้อมูล, User-Defined Routes (UUDR) สร้างเส้นทางการรับส่งข้อมูลของคุณใหม่กลับไปยังภายในองค์กร ('เส้นทางเริ่มต้น' 0.0.0/0/0) หรือไปยังบริษัทที่ใช้เครือข่าย
ถ้าคุณยังคงประสบปัญหาหลังจากลองใช้ขั้นตอนด้านบน โปรดระบุชื่อ VM และพอร์ต TCP ที่คุณพยายามส่งจดหมายเพื่อการกรองเพิ่มเติม

**เอกสารที่แนะนา**

[ข้อจํากัดและข้อเสนอแนะในการส่งอีเมลขาออกผ่านพอร์ต 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)