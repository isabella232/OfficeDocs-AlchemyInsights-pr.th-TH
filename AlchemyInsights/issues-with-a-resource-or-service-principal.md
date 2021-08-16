---
title: ปัญหาเกี่ยวกับทรัพยากรหรือบริการหลัก
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028095"
---
# <a name="issues-with-a-resource-or-service-principal"></a>ปัญหาเกี่ยวกับทรัพยากรหรือบริการหลัก

1. ถ้าคุณเพิ่งเริ่มต้นใช้งาน แอปพลิเคชันและบริการวัตถุหลักใน Azure Active Directory จะอธิบายการลงทะเบียนแอปพลิเคชัน วัตถุแอปพลิเคชัน และหลักของบริการใน[Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)วัตถุเหล่านั้น ถูกใช้งาน อย่างไร และวิธีที่เกี่ยวข้องกัน สถานการณ์สมมติตัวอย่างหลายผู้เช่ายังถูกนําเสนอเพื่อแสดงความสัมพันธ์ระหว่างวัตถุแอปพลิเคชันของแอปพลิเคชันและวัตถุหลักของบริการที่สอดคล้องกัน
2. คุณสามารถเรียนรู้เพิ่มเติมเกี่ยวกับความสัมพันธ์ระหว่างแอปพลิเคชันและหลักของบริการได้ด้วยการอ่าน[แอปพลิเคชันและวัตถุหลักของบริการใน](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)Azure Active Directory
3. [วิธีการ: ใช้พอร์ทัล](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)เพื่อสร้างแอปพลิเคชัน Azure AD และหลักบริการที่สามารถเข้าถึงทรัพยากรแสดงวิธีการสร้างแอปพลิเคชัน Azure Active Directory (Azure AD) ใหม่และหลักบริการที่สามารถใช้กับตัวควบคุมการเข้าถึงตามบทบาทได้
4. ด้วย [API หลักของบริการ](https://docs.microsoft.com/graph/api/resources/serviceprincipal)คุณสามารถจัดการอินสแตนซ์ของแอปพลิเคชันโดยทางโปรแกรม และควบคุมสิ่งที่แอปพลิเคชันสามารถดําเนินการภายในผู้เช่าของคุณ
5. [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.
6. [ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)จะเน้นความแตกต่างระหว่างแหล่งข้อมูล Azure AD Graphและแหล่งข้อมูลGraphของ Microsoft It shows resources that have different names or are not available; นอกจากนี้ยังเน้นแหล่งข้อมูลที่พร้อมใช้งานในเวอร์ชันเบต้าของ Microsoft Graph แต่ไม่อยู่ในเวอร์ชัน v1.0

**ปัญหาเกี่ยวกับผู้ใช้ที่เป็นแขก**

- [คู่มือเริ่มต้นใช้งานด่วน:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) เพิ่มผู้ใช้ที่เป็นผู้ใช้ภายนอกลงในไดเรกทอรีของคุณในพอร์ทัล Azure แสดงวิธีการเพิ่มผู้ใช้ที่เป็นผู้ใช้ภายนอกใหม่ในไดเรกทอรี Azure AD ผ่านพอร์ทัล Azure ส่งคําเชิญ และดูลักษณะของกระบวนการแลกใช้คําเชิญของผู้ใช้ภายนอก
- [บทช่วยสอน: สร้างโฟลว์ผู้ใช้Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows)แสดงวิธีการสร้างโฟลว์ผู้ใช้ที่แนะนาโดยใช้พอร์ทัล Azure ถ้าคุณมองหาข้อมูลเกี่ยวกับวิธีตั้งค่าโฟลว์รหัสผ่านเจ้าของทรัพยากร (ROPC) ในแอปพลิเคชันของคุณ ให้ดู กําหนดค่าโฟลว์ข้อมูลรับรองรหัสผ่านเจ้าของทรัพยากรใน Azure AD B2C
