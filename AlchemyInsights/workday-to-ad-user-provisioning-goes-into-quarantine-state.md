---
title: วันงานในการเตรียมใช้งานผู้ใช้ AD เข้าสู่สถานะการกักกัน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482906"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>การเตรียมใช้งานผู้ใช้ของวันงานไปยัง AD เข้าสู่สถานะการกักกัน

**วันงานในการเตรียมใช้งานผู้ใช้ AD เข้าสู่สถานะการกักกัน และไม่มีการสร้างผู้ใช้ใน AD**

วันงานเป็นงานการเตรียมใช้งานผู้ใช้ AD ได้เข้าสู่สถานะการกักกัน และบันทึกการตรวจสอบแสดงเหตุการณ์ความล้มเหลวในการส่งออกด้วยข้อผิดพลาดข้อความแสดงข้อผิดพลาด **: OperationsError-SvcErr: มีข้อผิดพลาดการดําเนินการเกิดขึ้น ไม่มีการกําหนดค่าการอ้างอิงแบบเหนือชั้นของบริการไดเรกทอรี บริการไดเรกทอรีจึงไม่สามารถออกการอ้างอิงไปยังวัตถุที่อยู่ภายนอกฟอเรสต์** นี้ ข้อผิดพลาดนี้มักจะแสดงขึ้นถ้า Active Directory Container OU ไม่ได้ตั้งค่าอย่างถูกต้อง หรือมีปัญหากับการแมปนิพจน์ที่ใช้ **กับ parentDistinguishedName**

ตรวจสอบค่าเริ่มต้น OU **for New Users** parameter for typos ตรวจสอบให้แน่ใจว่ามี OU ที่ระบุอยู่แล้วใน AD ของคุณ ถ้าคุณใช้ **ParentDistinguishedName** ในการแมปแอตทริบิวต์ ตรวจสอบให้แน่ใจว่าค่านี้ประเมินเป็นคอนเทนเนอร์ที่รู้จักภายในโดเมน AD เสมอ ตรวจสอบเหตุการณ์การส่งออกในบันทึกการตรวจสอบเพื่อดูค่าที่สร้างขึ้น

For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

