---
title: กำหนดค่า LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885580"
---
# <a name="configure-ldap"></a><span data-ttu-id="467c6-102">กำหนดค่า LDAP</span><span class="sxs-lookup"><span data-stu-id="467c6-102">Configure LDAP</span></span>

<span data-ttu-id="467c6-103">เมื่อต้องการกำหนดค่า LDAP ให้ทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="467c6-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="467c6-104">ตรวจสอบสถานภาพโดเมนของคุณบน[พอร์ทัล Azure](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="467c6-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="467c6-105">ตรวจสอบให้แน่ใจว่าการสมัครใช้งาน Azure AD ที่ถูกต้องจะพร้อมใช้งานและบริการโดเมน AD Azure ได้ถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="467c6-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="467c6-106">ใบรับรองที่จำเป็นต้องใช้ในการเปิดใช้งาน LDAP ที่ปลอดภัยต้องได้รับจากผู้ให้บริการออกใบรับรองสาธารณะที่เชื่อถือได้หรือเป็นใบรับรองแบบลงนามด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="467c6-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="467c6-107">ตรวจสอบให้แน่ใจว่าใบรับรองเป็นไปตาม [แนวทาง](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)ที่จำเป็น</span><span class="sxs-lookup"><span data-stu-id="467c6-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="467c6-108">**ใบรับรองที่ไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="467c6-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="467c6-109">เมื่อต้องการต่ออายุใบรับรองให้ทำตามขั้นตอนในการสร้างใบรับรองและ reupload ใหม่:[กำหนดค่า LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="467c6-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="467c6-110">เมื่อต้องการแก้ไขปัญหาที่ทราบเกี่ยวกับการแจ้งเตือน LDAP ที่ปลอดภัยในบริการโดเมนของ active directory ของ Azure ให้ดูที่[แก้ไขการแจ้งเตือนของ ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="467c6-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
