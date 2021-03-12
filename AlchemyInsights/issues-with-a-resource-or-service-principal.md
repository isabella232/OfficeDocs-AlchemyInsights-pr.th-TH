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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714462"
---
# <a name="issues-with-a-resource-or-service-principal"></a>ปัญหาเกี่ยวกับทรัพยากรหรือบริการหลัก

1. ถ้าคุณเพิ่งเริ่มต้นใช้งาน แอปพลิเคชันและบริการวัตถุหลักใน [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) จะอธิบายการลงทะเบียนแอปพลิเคชัน วัตถุแอปพลิเคชัน และหลักของบริการใน Azure Active Directory: สิ่งที่ถูกใช้งาน และวิธีที่วัตถุเหล่านั้นเกี่ยวข้องกัน สถานการณ์สมมติตัวอย่างหลายผู้เช่าจะแสดงเพื่อแสดงความสัมพันธ์ระหว่างวัตถุแอปพลิเคชันของแอปพลิเคชันและวัตถุหลักของบริการที่สอดคล้องกัน
2. คุณสามารถเรียนรู้เพิ่มเติมเกี่ยวกับความสัมพันธ์ระหว่างแอปพลิเคชันและหลักของบริการได้โดยการอ่าน[แอปพลิเคชันและวัตถุหลักของบริการใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [วิธีการ:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) ใช้พอร์ทัลเพื่อสร้างแอปพลิเคชัน Azure AD และหลักของบริการที่สามารถเข้าถึงทรัพยากรแสดงวิธีการสร้างแอปพลิเคชันและบริการหลักของ Azure Active Directory (Azure AD) ใหม่ที่สามารถใช้กับตัวควบคุมการเข้าถึงตามบทบาทได้
4. ด้วย [API หลักของบริการ](https://docs.microsoft.com/graph/api/resources/serviceprincipal)คุณสามารถจัดการอินสแตนซ์ของแอปพลิเคชันโดยทางโปรแกรมและควบคุมสิ่งที่แอปพลิเคชันสามารถดําเนินการภายในผู้เช่าของคุณ
5. [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.
6. [ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) จะเน้นความแตกต่างระหว่าง Azure AD Graph และแหล่งข้อมูล Microsoft Graph ซึ่งจะแสดงทรัพยากรที่มีชื่อแตกต่างกันหรือไม่พร้อมใช้งาน นอกจากนี้ยังเน้นแหล่งข้อมูลที่พร้อมใช้งานใน Microsoft Graph เวอร์ชันเบต้า แต่ไม่ใช่ในเวอร์ชัน v1.0

**ปัญหาเกี่ยวกับผู้ใช้ที่เป็นผู้ใช้ภายนอก**

- [การเริ่มต้นใช้งานด่วน:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) เพิ่มผู้ใช้ที่เป็นผู้ใช้ภายนอกลงในไดเรกทอรีในพอร์ทัล Azure แสดงวิธีการเพิ่มผู้ใช้ที่เป็นผู้ใช้ภายนอกใหม่ลงในไดเรกทอรี Azure AD ของคุณผ่านพอร์ทัล Azure ส่งคําเชิญ และดูลักษณะของกระบวนการแลกใช้คําเชิญของผู้ใช้ที่เป็นผู้ใช้ภายนอก
- [บทช่วยสอน: สร้างโฟลว์ผู้ใช้ใน Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) แสดงวิธีการสร้างโฟลว์ผู้ใช้ที่แนะนาโดยใช้พอร์ทัล Azure ถ้าคุณมองหาข้อมูลเกี่ยวกับวิธีตั้งค่าโฟลว์รหัสผ่านเจ้าของทรัพยากร (ROPC) ในแอปพลิเคชันของคุณ ให้ดู การกําหนดค่าโฟลว์ข้อมูลตัวของรหัสผ่านเจ้าของทรัพยากรใน Azure AD B2C
