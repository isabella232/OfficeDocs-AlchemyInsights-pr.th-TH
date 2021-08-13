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
ms.openlocfilehash: dc2068bbfde7b633e75b3d42f597cee8e4e5f5a72fbf22ebd6c2d0b768945dc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061667"
---
# <a name="scim-provisioning-issue"></a>ปัญหาการเตรียมใช้งาน SCIM

การเตรียมใช้งานโดยอัตโนมัติ หมายถึงการสร้างข้อมูลเฉพาะตัวผู้ใช้และบทบาทในแอปพลิเคชันระบบคลาวด์ที่ผู้ใช้ต้องเข้าถึง นอกจากการสร้างข้อมูลเฉพาะตัวของผู้ใช้แล้ว การเตรียมใช้งานโดยอัตโนมัติยังมีการบํารุงรักษาและการเอาข้อมูลเฉพาะตัวของผู้ใช้ออกเป็นสถานะหรือการเปลี่ยนแปลงบทบาท ก่อนที่คุณจะเริ่มการปรับใช้ คุณสามารถตรวจทาน[วิธีการเตรียมใช้งานงาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)เพื่อเรียนรู้วิธีการเตรียมใช้งาน Azure Active Directory (AD) และรับข้อแนะนะการกําหนดค่า

ในฐานะนักพัฒนาแอปพลิเคชัน คุณสามารถใช้ System for Cross-Domain Identity Management (SCIM) User Management API เพื่อเปิดใช้งานการเตรียมใช้งานผู้ใช้และกลุ่มโดยอัตโนมัติระหว่างแอปพลิเคชันของคุณและ Azure AD บทความ [สร้างจุดสิ้นสุด SCIM และกําหนดค่าการเตรียมใช้งาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) ผู้ใช้ด้วย Azure AD จะอธิบายวิธีการสร้างจุดสิ้นสุด SCIM และรวมกับบริการการเตรียมใช้งาน Azure AD



