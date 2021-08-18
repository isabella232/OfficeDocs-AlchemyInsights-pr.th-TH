---
title: สถานะโดเมน - ไม่ได้เลือกบริการไว้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326596"
---
# <a name="domain-status---no-services-selected"></a>สถานะโดเมน - ไม่ได้เลือกบริการไว้

ไม่ได้ **เลือกบริการ** ไว้หมายความว่าคุณยังไม่ได้เลือกบริการใดๆ Microsoft 365 เช่น Exchange Online, Skype for Business หรือ Intuned และการจัดการอุปกรณ์เคลื่อนที่Microsoft 365เพื่อใช้กับโดเมนแบบปรับแต่งเองของคุณ ถ้าคุณใช้งาน Exchange Hybrid (ภายในExchangeองค์กรที่มี Exchange Online) หรือการกรองสแปมภายนอกด้วย Exchange และไม่มีบริการของ Microsoftอื่นๆ คุณสามารถละเว้นข้อความนี้ สถานะความสมบูรณ์ของโดเมนจะพร้อมใช้งานเฉพาะโดเมนที่เชื่อมต่อกับบริการโดยตรงเท่านั้น

เมื่อต้องการเลือกบริการต่างๆ ให้กับโดเมนของคุณ:

1. จาก **การตั้งค่า**  >  [**โดเมน**](https://admin.microsoft.com/Adminportal/Home)ของคุณ ให้เลือกกล่องที่อยู่ถัดจากโดเมนที่มีข้อความสถานะ **ไม่มีบริการ** ที่เลือก
1. เลือก **จัดการ DNS** เพื่อเริ่มตัวช่วยสร้างการตั้งค่าโดเมน
    - ถ้าคุณเลือก **เพิ่มระเบียน DNS ของคุณเอง** ตรวจสอบให้แน่ใจว่าได้เลือกบริการเมื่อได้รับพร้อมท์ บริการเพิ่มเติมอาจพร้อมใช้งานภายใต้ **ตัวเลือก** ขั้นสูง
    - ถ้าคุณเลือก ให้ **ไมโครซอฟท์เพิ่มระเบียน DNS ของคุณ** หรือ **ตัวเลือก** เพิ่มเติม ตั้งค่าบริการออนไลน์ของฉันให้ฉัน บริการ  >  ที่พร้อมใช้งานทั้งหมดจะถูกแนะนาและเลือกโดยอัตโนมัติ
1. ใช้งานตัวช่วยสร้างต่อไปเพื่อเสร็จสิ้นการตั้งค่า DNS และตัวเลือกบริการของคุณ
 
For additional help setting up your domain, see [Add DNS records to connect your domain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

