---
title: SAML Assertions (โทเค็น)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109259"
---
# <a name="saml-assertions-tokens"></a>SAML Assertions (โทเค็น)

1. โทเค็น Security Assertions Markup Language (SAML) เป็นการแสดง XML ของการอ้างสิทธิ์ ตามค่าเริ่มต้น โทเค็น SAML Windows Communication Foundation (WCF) จะใช้ในสถานการณ์ด้านความปลอดภัยแบบติดต่อภายนอก For more information, see [SAML tokens and claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. ไคลเอ็นต์แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโทเค็นความปลอดภัยหลายชนิดในการประมวลผลของโฟลว์การรับรองความถูกต้องแต่ละรายการ [การอ้างอิงการอ้างสิทธิ์โทเค็น SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) จะอธิบายรูปแบบ คุณลักษณะด้านความปลอดภัย และเนื้อหาของโทเค็น SAML 2.0
3. Follow the guidance in [Configurable token lifetimes in แพลตฟอร์มข้อมูลประจําตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.
4. Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.
5. ใน Azure AD คุณสามารถตั้งค่าตัวเลือกการลงชื่อใบรับรองและอัลกอริทึมการเซ็นชื่อใบรับรองได้ For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
