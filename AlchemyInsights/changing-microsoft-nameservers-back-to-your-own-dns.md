---
title: การเปลี่ยนจากเซิร์ฟเวอร์ชื่อ Microsoft กลับเป็นการจัดการระเบียน DNS ของคุณเอง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506975"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>การเปลี่ยนจากเซิร์ฟเวอร์ชื่อ Microsoft กลับเป็นการจัดการระเบียน DNS ของคุณเอง

คุณเคยเปลี่ยนระเบียน NS ให้ชี้ไปยัง Microsoft (ns1.bdm.microsoftonline.com) แต่ตอนนี้ได้ตัดสินใจจัดการระเบียน DNS ของคุณเองแล้ว:

ที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณ ให้เปลี่ยนเนมเซิร์ฟเวอร์กลับไปเป็นบริษัทจดทะเบียนหรือการตั้งค่าก่อนหน้าของคุณ ถ้าคุณไม่คุ้นเคยกับ DNS ให้ติดต่อฝ่ายสนับสนุนที่บริษัทจดทะเบียนโดเมน โปรดทราบว่าการเปลี่ยนแปลงเซิร์ฟเวอร์ชื่ออาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่ 

1. ใน Microsoft 365 Admin Portal ให้ไปที่ **การตั้งค่า**  >  [**โดเมน**](https://admin.microsoft.com/Adminportal/Home#/Domains)ของคุณ เลือกกล่องกาเครื่องหมายที่อยู่ถัดจากโดเมน แล้วเลือก **จัดการ DNS** 

2. ในตัวช่วยสร้าง ให้เลือก **เพิ่มระเบียน DNS ของคุณเอง** และกรอกตัวช่วยสร้างให้เสร็จสมบูรณ์ การเปลี่ยนแปลงนี้จะเปลี่ยนวิธีการที่ DNS ของคุณได้รับการจัดการ และอนุญาตให้คุณเพิ่มระเบียน DNS แบบปรับแต่งเองที่ต้องใช้เพื่อสนับสนุนบริการที่เลือกของคุณ

หรือ ถ้าคุณเปลี่ยนระเบียนเนมเซิร์ฟเวอร์ของคุณไปยังไมโครซอฟท์และมีเว็บไซต์ คุณสามารถเพิ่มระเบียน DNS ของเว็บไซต์แทนการเปลี่ยนเนมเซิร์ฟเวอร์กลับได้ For more information, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


