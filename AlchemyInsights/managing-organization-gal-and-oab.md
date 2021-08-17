---
title: การจัดการสมุดรายชื่อส่วนกลางขององค์กรและสมุดรายชื่อแบบออฟไลน์
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
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042181"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>การจัดการสมุดรายชื่อส่วนกลาง (GAL) และสมุดรายชื่อแบบออฟไลน์ (OAB) ขององค์กร

สมุดรายชื่อส่วนกลาง (GAL) คือรายการของวัตถุที่เปิดใช้งานจดหมาย (ชนิดของผู้รับใดๆ ที่สามารถรับอีเมล) ในองค์กร GAL หนึ่งรายการจะถูกสร้างขึ้นโดยอัตโนมัติในทุกองค์กร คุณสามารถสร้าง GALs เพิ่มเติมเพื่อแยกผู้ใช้ตามองค์กรหรือสถานที่ แต่ผู้ใช้คนเดียวสามารถดูและใช้ GAL ได้ทีละหนึ่งรายการเท่านั้น

ไคลเอ็นต์อีเมลบางไคลเอ็นต์ เช่น Outlookไคลเอ็นต์Windows ให้ดาวน์โหลด GAL เพื่อใช้งานแบบออฟไลน์ ซึ่งเรียกว่าสมุดรายชื่อแบบออฟไลน์ (OAB) ใน Exchange ออนไลน์ OAB จะถูกอัปเดตหนึ่งครั้งทุกๆ 8 ชั่วโมงเท่านั้น และลูกค้าต้องดาวน์โหลดเพื่ออัปเดตสําเนา OAB ภายในเครื่องของตน การเปลี่ยนแปลงใดๆ ของผู้รับจะต้องมองเห็นได้ใน GAL ก่อนเพื่อเปลี่ยนเป็น OAB ในภายหลัง

ต่อไปนี้คือขั้นตอน GAL และ OAB ที่ใช้บ่อย:

- ด้วยเหตุผลหลายประการ คุณอาจต้องการซ่อนวัตถุบางอย่างจาก GAL โปรดดูที่ [ซ่อนผู้รับจากรายการ](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)ที่อยู่
- If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [สร้างสมุดรายชื่อส่วนกลางใน Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)และเมื่อต้องการเรียนรู้วิธีใช้งานกับสิทธิ์ GAL ให้ดู[รายการที่อยู่Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) โปรดทราบว่าถ้าคุณสร้าง GALs ใหม่ คุณอาจต้องการสร้าง OAB ใหม่ ดู [กระบวนงานสมุดรายชื่อ](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)แบบออฟไลน์
