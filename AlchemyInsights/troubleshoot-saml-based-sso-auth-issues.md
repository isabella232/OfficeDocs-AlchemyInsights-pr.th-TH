---
title: แก้ไขปัญหาการรับรองความถูกต้อง SSO แบบใช้ SAML
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "9409"
ms.openlocfilehash: c053e252edfcc51c95214c4bff4aded2bded2e23
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695665"
---
# <a name="troubleshoot-saml-based-sso-authentication-issues"></a><span data-ttu-id="1e708-102">แก้ไขปัญหาการรับรองความถูกต้อง SSO แบบใช้ SAML</span><span class="sxs-lookup"><span data-stu-id="1e708-102">Troubleshoot SAML-based SSO authentication issues</span></span>

<span data-ttu-id="1e708-103">ผู้ใช้ส่วนใหญ่สามารถแก้ไขปัญหาการรับรองความถูกต้อง SSO แบบ SAML โดยใช้ขั้นตอนที่แนะนําต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1e708-103">Most users are able to resolve their SAML-based SSO authentication issues using the following recommended steps:</span></span>

<span data-ttu-id="1e708-104">**ขั้นตอนที่แนะนา**</span><span class="sxs-lookup"><span data-stu-id="1e708-104">**Recommended Steps**</span></span>
1. <span data-ttu-id="1e708-105">ค้นหา [ข้อมูลรหัสข้อผิดพลาด](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information)ปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="1e708-105">Lookup [current error code information](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information).</span></span>
1. <span data-ttu-id="1e708-106">ดู [การลงชื่อเข้าระบบครั้งเดียวโดยใช้ DEBUG SAML ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) เพื่อแก้ไขข้อผิดพลาดการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1e708-106">See [Debug SAML-based single sign-on to applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) to resolve authentication errors.</span></span>
1. <span data-ttu-id="1e708-107">ดูบทความ โพรโทคอล [SAML Sign-On เดี่ยว](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) เพื่อเรียนรู้เกี่ยวกับการร้องขอการรับรองความถูกต้อง SAML 2.0 และการตอบกลับที่ Azure Active Directory (Azure AD) สนับสนุน Sign-On เดี่ยว (SSO)</span><span class="sxs-lookup"><span data-stu-id="1e708-107">Refer to the article, [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) to learn about the SAML 2.0 authentication requests and responses that Azure Active Directory (Azure AD) supports for Single Sign-On (SSO).</span></span>


