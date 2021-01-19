---
title: การกำหนดค่าและการแก้ไขปัญหาการอ้างสิทธิ์ของ SAML
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
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901292"
---
# <a name="configure-and-troubleshoot-saml-claims"></a>การกำหนดค่าและการแก้ไขปัญหาการอ้างสิทธิ์ของ SAML

เมื่อต้องการกำหนดค่าและแก้ไขปัญหาการอ้างสิทธิ์ SAML:

1. ทำตามขั้นตอนที่ระบุไว้ใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) เพื่อกำหนดค่าการอ้างสิทธิ์บทบาทที่ออกในโทเค็น SAML สำหรับแอปพลิเคชันสำหรับองค์กร
2. ทำตามขั้นตอนใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) เพื่อกำหนดค่าการอ้างสิทธิ์ที่ออกในโทเค็น SAML สำหรับแอปพลิเคชันสำหรับองค์กร
3. ทำตามขั้นตอนใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) เพื่อกำหนดค่าการอ้างสิทธิ์ที่ออกมาในโทเค็นสำหรับแอปที่เฉพาะเจาะจงในผู้เช่า
4. อ่าน [บทความนี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) เพื่อทำความเข้าใจเกี่ยวกับการทำงานกับแอปพลิเคชันการอ้างสิทธิ์ในพร็อกซีของแอปพลิเคชัน