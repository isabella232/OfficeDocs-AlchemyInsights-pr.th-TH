---
title: กําหนดค่าและแก้ไขปัญหาการอ้างสิทธิ์ SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 20aede85988e509a055724cc570c249abe8ea7950aa04e3f9d728d0b4abf885c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044575"
---
# <a name="configure-and-troubleshoot-saml-claims"></a>กําหนดค่าและแก้ไขปัญหาการอ้างสิทธิ์ SAML

เมื่อต้องการกําหนดค่าและแก้ไขปัญหาการอ้างสิทธิ์ SAML:

1. Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.
2. Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.
3. Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in token for a specific app in a tenant.
4. อ่านบทความ [นี้เพื่อ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) เข้าใจการใช้งานได้กับแอปที่รับรู้การอ้างสิทธิ์ในพร็อกซีแอปพลิเคชัน