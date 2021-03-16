---
title: แก้ไขปัญหารหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9367"
- "9004357"
ms.openlocfilehash: 805a85ffd47e14295c375fc415301570de22bfd8
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816364"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-error-codes-and-messages"></a><span data-ttu-id="c2aa0-102">แก้ไขปัญหารหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="c2aa0-102">Troubleshoot Seamless Single Sign-on (SSO) error codes and messages</span></span>

<span data-ttu-id="c2aa0-103">เมื่อต้องการแก้ไขรหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c2aa0-103">To resolve Seamless Single Sign-on (SSO) error codes and messages, perform the following steps:</span></span>

1. <span data-ttu-id="c2aa0-104">ตรวจสอบและแก้ไขข้อผิดพลาด SSO โดยไปที่[รายงานกิจกรรมการลงชื่อเข้าใช้ในพอร์ทัล Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)</span><span class="sxs-lookup"><span data-stu-id="c2aa0-104">Review and troubleshoot SSO errors by going to the [Sign-in activity reports in the Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins).</span></span>
2. <span data-ttu-id="c2aa0-105">ดู [การแก้ไขปัญหาการ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) ลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ Azure Active Directory - บทความนี้ช่วยให้คุณค้นหาข้อมูลการแก้ไขปัญหาทั่วไปเกี่ยวกับ Azure Active Directory (Azure AD) การเข้าสู่ระบบครั้งเดียวอย่างราบรื่น (SSO อย่างราบรื่น Sign-On)</span><span class="sxs-lookup"><span data-stu-id="c2aa0-105">See [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>
3. <span data-ttu-id="c2aa0-106">ดู [การรับรองความถูกต้องของ Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) และรหัสข้อผิดพลาดการอนุญาต - บทความนี้ช่วยให้คุณค้นหาข้อมูลเกี่ยวกับรหัสข้อผิดพลาด AADSTS ที่ส่งกลับจากบริการโทเค็นความปลอดภัย (STS) ของ Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="c2aa0-106">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) - This article helps you find information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS).</span></span> <span data-ttu-id="c2aa0-107">บทความนี้ยังช่วยให้คุณค้นหารายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราวที่แนะน</span><span class="sxs-lookup"><span data-stu-id="c2aa0-107">This article also helps you find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="c2aa0-108">[ถามตอบ&ของ Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - ดูบทความนี้เพื่อดูข้อมูลเกี่ยวกับการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="c2aa0-108">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - See this article for information on making feature requests or asking technical questions about Seamless SSO.</span></span>

