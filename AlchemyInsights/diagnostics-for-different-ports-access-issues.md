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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036806"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>การวินิจฉัยปัญหาการเข้าถึงพอร์ตต่างๆ

เมื่อต้องการแก้ไขปัญหาการเข้าถึงพอร์ตต่างๆ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. หยุด/จัดการเครื่องเสมือน (VM) จากพอร์ทัล เริ่ม VM ใหม่ และทดสอบอีกครั้ง 
2. ตรวจสอบการตั้งค่าเครือข่ายของ VM ของคุณเพื่อตรวจสอบว่าคุณมีการรับส่งข้อมูลบล็อกกลุ่มความปลอดภัยของเครือข่าย (NSG) หรือไม่ คุณยังสามารถใช้เครื่องมือตรวจสอบ [IP ของ Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) เพื่อตรวจสอบ NSGs ที่บล็อกการรับส่งข้อมูล, เส้นทาง User-Defined (UUDR) สร้างเส้นทางการรับส่งข้อมูลของคุณใหม่ไปยังภายในองค์กร ('Default Route' 0.0.0.0/0) หรือกับผู้ตรวจสอบเครือข่าย
ถ้าคุณยังคงพบปัญหาหลังจากลองปฏิบัติตามขั้นตอนด้านบน โปรดระบุชื่อ VM และพอร์ต TCP ที่คุณพยายามส่งจดหมายเพื่อแก้ปัญหาเพิ่มเติม

**เอกสารที่แนะนา**

[ข้อจํากัดและข้อเสนอแนะในการส่งอีเมลขาออกผ่านพอร์ต 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)