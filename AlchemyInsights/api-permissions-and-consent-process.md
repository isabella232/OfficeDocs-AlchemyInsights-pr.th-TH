---
title: สิทธิ์ API และกระบวนการให้ความยินยอม
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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405443"
---
# <a name="api-permissions-and-consent-process"></a>สิทธิ์ API และกระบวนการให้ความยินยอม

เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม [การอ้างอิงสิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์

**การตั้งค่าหรืออัปเดตหลักของบริการ**

- [สร้าง serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - บทความนี้จะแสดงวิธีการสร้างวัตถุ servicePrincipal ใหม่
- [สร้างบัญชีหลักของ& Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) ในพอร์ทัล - บทความนี้แสดงวิธีการสร้างแอปพลิเคชัน Azure Active Directory (Azure AD) ใหม่และหลักบริการที่สามารถใช้กับตัวควบคุมการเข้าถึงตามบทบาท
- [แอป&](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) หลักบริการหลักใน Azure AD - บทความนี้อธิบายการลงทะเบียนแอปพลิเคชัน วัตถุแอปพลิเคชัน และหลักของบริการใน Azure Active Directory: สิ่งที่พวกเขาใช้ และวิธีการที่เกี่ยวข้องกัน

**เพิ่มหรืออัปเดตการลงทะเบียนแอปและให้ความยินยอมจากผู้ดูแลระบบ**

- [สร้างการลงทะเบียนแอป](https://docs.microsoft.com/graph/api/application-post-applications) - บทความนี้จะแสดงวิธีการสร้างวัตถุแอปพลิเคชันใหม่
- [อัปเดตการลงทะเบียนแอป - สิทธิ์ API](https://docs.microsoft.com/graph/api/application-update) - บทความนี้จะแสดงวิธีการอัปเดตคุณสมบัติของวัตถุแอปพลิเคชัน
- [ให้ความยินยอมจาก](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) ผู้ดูแลระบบ - ในการยินยอมของผู้ดูแลระบบและความยินยอมทั่วไป เราต้องการให้ผู้ดูแลระบบอนุญาตการยินยอมอย่างชัดเจน
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - คอนเทนเนอร์การจัดการบทบาทเพื่อนิยามบทบาทที่เป็นหนึ่งเดียวและการมอบหมายบทบาทให้กับผู้ให้บริการ RBAC ของ Microsoft 365 ที่สนับสนุนหลักจํานวนมากและมีหลายขอบเขตในการมอบหมายบทบาทเดียว ซึ่งแตกต่างจากชนิดทรัพยากร *rbacApplication* Microsoft Intun1 เป็นตัวอย่างของผู้ให้บริการ RBAC ดังกล่าว การมอบหมายบทบาทใน Intun1 สามารถมีอาร์เรย์ของชื่อหลักและอาร์เรย์ของกลุ่มขอบเขตได้ **ค่านี้เป็นรุ่นเบต้า หมายความว่ายังอยู่ในช่วงการพัฒนาและไม่แนะนนะให้ใช้งานในการผลิต**
