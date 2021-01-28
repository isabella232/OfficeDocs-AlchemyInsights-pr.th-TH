---
title: ปัญหาเกี่ยวกับการอ้างสิทธิ์และแอตทริบิวต์โทเค็น
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036078"
---
# <a name="issues-with-token-claims-and-attributes"></a>ปัญหาเกี่ยวกับการอ้างสิทธิ์และแอตทริบิวต์โทเค็น

**อัปเดต กําหนดค่า หรือเอาการอ้างสิทธิ์โทเค็นออก**

1. ด้วยการใช้ Azure Active Directory (Azure AD) คุณสามารถปรับแต่งชนิดการอ้างสิทธิ์ของ [บทบาทใน](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) โทเค็นตอบกลับที่คุณได้รับหลังจากที่คุณอนุญาตแอปได้
2. นักพัฒนาแอปพลิเคชันสามารถใช้การอ้างสิทธิ์เพิ่มเติมในแอปพลิเคชัน Azure AD เพื่อระบุการอ้างสิทธิ์ที่พวกเขาต้องการในโทเค็นที่ส่งไปยังแอปพลิเคชันของพวกเขา For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [กําหนดค่าการอ้างสิทธิ์กลุ่มของแอปพลิเคชันด้วย Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. ถ้าใช้การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่นในแอปพลิเคชันของคุณ ให้ดู[การอ้างสิทธิ์แบบปรับแต่งที่ออกในโทเค็น SAML ของแอปพลิเคชันขององค์กร](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**การอ้างสิทธิ์การแมปแอตทริบิวต์**

1. To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. แอตทริบิวต์ส่วนขยาย Schema ไดเรกทอรีมีวิธีการจัดเก็บข้อมูลเพิ่มเติมใน Azure Active Directory บนวัตถุผู้ใช้และวัตถุไดเรกทอรีอื่นๆ เช่น กลุ่ม รายละเอียดผู้เช่า หลักบริการ เฉพาะแอตทริบิวต์ส่วนขยายบนวัตถุของผู้ใช้เท่านั้นที่สามารถใช้ในการอ้างสิทธิ์ไปยังแอปพลิเคชันได้ [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.

ดูข้อมูลเพิ่มเติมเกี่ยวกับการอ้างสิทธิ์โทเค็นที่:

- [อ้างสิทธิ์ในโทเค็นการเข้าถึง](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [การอ้างสิทธิ์ในid_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [การอ้าง](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) สิทธิ์ที่คุณสามารถคาดหวังในโทเค็น ID และโทเค็นการเข้าถึงที่ออกโดย Azure AD B2C
- [การอ้างอิงการอ้างสิทธิ์โทเค็น SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
