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
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="ad3c6-102">การกำหนดค่าและการแก้ไขปัญหาการอ้างสิทธิ์ของ SAML</span><span class="sxs-lookup"><span data-stu-id="ad3c6-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="ad3c6-103">เมื่อต้องการกำหนดค่าและแก้ไขปัญหาการอ้างสิทธิ์ SAML:</span><span class="sxs-lookup"><span data-stu-id="ad3c6-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="ad3c6-104">ทำตามขั้นตอนที่ระบุไว้ใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) เพื่อกำหนดค่าการอ้างสิทธิ์บทบาทที่ออกในโทเค็น SAML สำหรับแอปพลิเคชันสำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="ad3c6-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="ad3c6-105">ทำตามขั้นตอนใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) เพื่อกำหนดค่าการอ้างสิทธิ์ที่ออกในโทเค็น SAML สำหรับแอปพลิเคชันสำหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="ad3c6-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="ad3c6-106">ทำตามขั้นตอนใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) เพื่อกำหนดค่าการอ้างสิทธิ์ที่ออกมาในโทเค็นสำหรับแอปที่เฉพาะเจาะจงในผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="ad3c6-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="ad3c6-107">อ่าน [บทความนี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) เพื่อทำความเข้าใจเกี่ยวกับการทำงานกับแอปพลิเคชันการอ้างสิทธิ์ในพร็อกซีของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="ad3c6-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>