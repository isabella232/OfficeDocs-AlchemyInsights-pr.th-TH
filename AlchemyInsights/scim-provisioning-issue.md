---
title: ปัญหาการเตรียมใช้งาน SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949950"
---
# <a name="scim-provisioning-issue"></a>ปัญหาการเตรียมใช้งาน SCIM

การจัดเตรียมอัตโนมัติอ้างอิงถึงการสร้างข้อมูลเฉพาะตัวของผู้ใช้และบทบาทในแอปพลิเคชัน cloud ที่ผู้ใช้ต้องการเข้าถึง นอกเหนือจากการสร้างข้อมูลเฉพาะตัวของผู้ใช้การเตรียมใช้งานอัตโนมัติจะรวมถึงการบำรุงรักษาและการเอาข้อมูลประจำตัวของผู้ใช้ออกเป็นสถานะหรือบทบาทการเปลี่ยนแปลง ก่อนที่คุณจะเริ่มต้นการปรับใช้คุณสามารถตรวจสอบ [วิธีการเตรียมใช้งานการทำงาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) เพื่อเรียนรู้วิธีการเตรียมใช้งานการเตรียมใช้งานของ Azure active DIRECTORY (AD) และรับคำแนะนำในการกำหนดค่า

ในฐานะนักพัฒนาแอปพลิเคชันคุณสามารถใช้ API สำหรับการจัดการผู้ใช้ข้อมูลประจำตัวแบบข้ามโดเมน (SCIM) เพื่อเปิดใช้งานการเตรียมใช้งานอัตโนมัติของผู้ใช้และกลุ่มระหว่างแอปพลิเคชันของคุณและ Azure AD การ [สร้างจุดสิ้นสุด SCIM และกำหนดค่าการเตรียมใช้งานของผู้ใช้ด้วยบทความ AD Azure](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) จะอธิบายวิธีการสร้างจุดสิ้นสุด SCIM และรวมเข้ากับบริการการเตรียมใช้งาน Azure AD



