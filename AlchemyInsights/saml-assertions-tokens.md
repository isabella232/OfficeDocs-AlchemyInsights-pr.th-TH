---
title: การยืนยันของ SAML (โทเค็น)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885678"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="bc58a-102">การยืนยันของ SAML (โทเค็น)</span><span class="sxs-lookup"><span data-stu-id="bc58a-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="bc58a-103">โทเค็นภาษามาร์กอัปสิทธิ์การใช้งานของการรับรองความปลอดภัย (SAML) คือ XML ที่ใช้ในการอ้างสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="bc58a-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="bc58a-104">ตามค่าเริ่มต้นโทเค็น SAML ของ Windows ตสื่อสารมูลฐาน (WCF) ใช้ในสถานการณ์การรักษาความปลอดภัยที่ติดต่อกับภายนอกโทเค็นที่ออก</span><span class="sxs-lookup"><span data-stu-id="bc58a-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="bc58a-105">สำหรับข้อมูลเพิ่มเติมให้ดูที่[โทเค็นของ SAML และการอ้างสิทธิ์](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="bc58a-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="bc58a-106">แพลตฟอร์มสำหรับข้อมูลเฉพาะตัวของ Microsoft จะปล่อยโทเค็นความปลอดภัยหลายชนิดในการประมวลผลการรับรองความถูกต้องของแต่ละขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="bc58a-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="bc58a-107">การ[อ้างอิงการอ้างสิทธิ์โทเค็น saml](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)จะอธิบายรูปแบบลักษณะความปลอดภัยและเนื้อหาของโทเค็น๒.๐ของ saml</span><span class="sxs-lookup"><span data-stu-id="bc58a-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="bc58a-108">ทำตามคำแนะนำในการกำหนดค่าของโทเค็นที่สามารถกำหนดค่าได้ [ใน Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) เพื่อทำความเข้าใจวิธีการกำหนดค่าอายุการใช้งานของโทเค็น</span><span class="sxs-lookup"><span data-stu-id="bc58a-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="bc58a-109">ทำตามขั้นตอนที่ระบุไว้ใน [บทความนี้](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) เพื่อทำความเข้าใจเกี่ยวกับวิธีการกำหนดค่าการเข้ารหัสลับโทเค็นการ SAML AD ของ Azure</span><span class="sxs-lookup"><span data-stu-id="bc58a-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="bc58a-110">ใน Azure AD คุณสามารถตั้งค่าตัวเลือกการเซ็นชื่อใบรับรองและอัลกอริทึมการเซ็นชื่อใบรับรองได้</span><span class="sxs-lookup"><span data-stu-id="bc58a-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="bc58a-111">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตัวเลือกการเซ็นชื่อใบรับรองขั้นสูงในโทเค็น SAML สำหรับแอปแกลเลอรีใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="bc58a-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
