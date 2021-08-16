---
title: ปัญหาเกี่ยวกับการอ้างสิทธิ์โทเค็นและแอตทริบิวต์
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012903"
---
# <a name="issues-with-token-claims-and-attributes"></a>ปัญหาเกี่ยวกับการอ้างสิทธิ์โทเค็นและแอตทริบิวต์

**อัปเดต กําหนดค่า หรือเอาการอ้างสิทธิ์โทเค็นออก**

1. ด้วยการใช้Azure Active Directory (Azure AD) คุณสามารถปรับแต่งชนิดการ[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)อ้างสิทธิ์ของบทบาทในโทเค็นการตอบกลับที่คุณได้รับหลังจากที่คุณอนุมัติแอปได้
2. นักพัฒนาแอปพลิเคชันสามารถใช้การอ้างสิทธิ์เพิ่มเติมในแอปพลิเคชัน Azure AD ของพวกเขาเพื่อระบุว่าพวกเขาต้องการเรียกร้องใดในโทเค็นที่ส่งไปยังแอปพลิเคชันของพวกเขา For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [กําหนดค่าการอ้างสิทธิ์กลุ่มAzure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)รายการ
4. If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**การอ้างสิทธิ์การแมปแอตทริบิวต์**

1. To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. แอตทริบิวต์ส่วนขยาย Schema ไดเรกทอรีมีวิธีการจัดเก็บข้อมูลเพิ่มเติมAzure Active Directoryวัตถุผู้ใช้และวัตถุไดเรกทอรีอื่นๆ เช่น กลุ่ม รายละเอียดผู้เช่า หลักบริการ Only extension attributes on user objects can be used for emitting claims to applications. [การใช้แอตทริบิวต์ส่วนขยาย Schema ไดเรกทอรีในการอ้างสิทธิ์](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) จะอธิบายวิธีใช้แอตทริบิวต์ส่วนขยาย Schema ไดเรกทอรีเพื่อส่งข้อมูลผู้ใช้ไปยังแอปพลิเคชันในการเรียกร้องโทเค็น

For more information on token claims, see:

- [การอ้างสิทธิ์ในโทเค็นการเข้าถึง](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [การอ้างสิทธิ์ในid_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [การอ้าง](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) สิทธิ์ที่คุณสามารถคาดหวังในโทเค็น ID และโทเค็นการเข้าถึงที่ออกโดย Azure AD B2C
- [การอ้างอิงการอ้างสิทธิ์โทเค็น SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
