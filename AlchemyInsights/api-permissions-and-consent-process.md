---
title: สิทธิ์ของ API และกระบวนการยินยอม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932080"
---
# <a name="api-permissions-and-consent-process"></a>สิทธิ์ของ API และกระบวนการยินยอม

เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graphหรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม [การอ้างอิงGraphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference)จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft Graph API แต่ละรายการ นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์

**การตั้งค่าหรืออัปเดตหลักของบริการ**

- [สร้าง serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - บทความนี้แสดงวิธีการสร้างวัตถุ servicePrincipal ใหม่
- [สร้างแอป Azure AD &หลัก](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)บริการในพอร์ทัล - บทความนี้แสดงวิธีการสร้างแอปพลิเคชัน Azure Active Directory (Azure AD) ใหม่และหลักบริการที่สามารถใช้กับตัวควบคุมการเข้าถึงตามบทบาทได้
- [แอป&](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)หลักบริการใน Azure AD - บทความนี้อธิบายการลงทะเบียนแอปพลิเคชัน วัตถุแอปพลิเคชัน และหลักบริการใน Azure Active Directory: ข้อมูลเหล่านี้ วิธีใช้ และวิธีที่เกี่ยวข้องกัน

**เพิ่มหรืออัปเดตการลงทะเบียนแอปและให้ความยินยอมจากผู้ดูแลระบบ**

- [สร้างการลงทะเบียนแอป](https://docs.microsoft.com/graph/api/application-post-applications) - บทความนี้จะแสดงวิธีการสร้างวัตถุแอปพลิเคชันใหม่
- [อัปเดตการลงทะเบียนแอป - สิทธิ์ API](https://docs.microsoft.com/graph/api/application-update) - บทความนี้แสดงวิธีอัปเดตคุณสมบัติของวัตถุแอปพลิเคชัน
- [ให้ความยินยอมจาก](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) ผู้ดูแลระบบ - ในความยินยอมของผู้ดูแลระบบและความยินยอมโดยทั่วไป เราต้องการให้ผู้ดูแลระบบให้ความยินยอมอย่างชัดเจน
- [RBAC (รุ่นเบต้า)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - คอนเทนเนอร์การจัดการบทบาทเพื่อนิยามบทบาทแบบรวมและการมอบหมายบทบาทMicrosoft 365ผู้ให้บริการ RBAC ที่สนับสนุนหลักการหลักหลายขอบเขตและหลายขอบเขตในการมอบหมายบทบาทเดียว ซึ่งแตกต่างจาก *rbacApplication* resource type Microsoft Intuneเป็นตัวอย่างของผู้ให้บริการ RBAC ดังกล่าว การมอบหมายบทบาทใน Intun1 สามารถมีอาร์เรย์ของชื่อหลักและอาร์เรย์ของกลุ่มขอบเขตได้ **ซึ่งยังอยู่ในช่วงเบต้า ซึ่งหมายความว่าจะยังคงอยู่ในการพัฒนาและไม่แนะนนะให้ใช้งานในรุ่นการผลิต**
