---
title: วันการเตรียมใช้งานของผู้ใช้ AD เข้าสู่สถานะการกักกัน
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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036511"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>วันการเตรียมใช้งานของผู้ใช้ AD เข้าสู่สถานะการกักกัน

**วันงานในการเตรียมใช้งานผู้ใช้ AD เข้าสู่สถานะการกักกัน และไม่ได้สร้างผู้ใช้ใน AD**

งานการเตรียมใช้งานของผู้ใช้เป็น AD เข้าสู่สถานะการกักกันและบันทึกการตรวจสอบแสดงเหตุการณ์ความล้มเหลวของการส่งออกด้วยข้อความแสดงข้อผิดพลาด: **OperationsError-SvcErr: มีข้อผิดพลาดการดําเนินการเกิดขึ้น ไม่มีการกําหนดค่าการอ้างอิงแบบเหนือชั้นของบริการไดเรกทอรี บริการไดเรกทอรีจึงไม่สามารถออกการอ้างอิงไปยังวัตถุภายนอกฟอเรสต์** นี้ ข้อผิดพลาดนี้มักจะแสดงขึ้นถ้า Active Directory Container OU ไม่ได้ตั้งค่าอย่างถูกต้อง หรือถ้ามีปัญหากับการแมปนิพจน์ที่ใช้กับ **parentDistinguishedName**

ตรวจสอบค่าเริ่มต้น OU for **New Users** parameter for typos ตรวจสอบให้แน่ใจว่ามี OU ที่ระบุอยู่แล้วใน AD ของคุณ ถ้าคุณใช้ **parentDistinguishedName** ในการแมปแอตทริบิวต์ ตรวจสอบให้แน่ใจว่าค่านี้ประเมินเป็นคอนเทนเนอร์ที่รู้จักภายในโดเมน AD เสมอ ตรวจสอบเหตุการณ์ ส่งออก ในบันทึกการตรวจสอบเพื่อดูค่าที่สร้างขึ้น

For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

