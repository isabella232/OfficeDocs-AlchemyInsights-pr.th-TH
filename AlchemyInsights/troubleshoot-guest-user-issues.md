---
title: แก้ไขปัญหาผู้ใช้ที่เป็นแขก
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939398"
---
# <a name="troubleshoot-guest-user-issues"></a>แก้ไขปัญหาผู้ใช้ที่เป็นแขก

1. สําหรับแนวทางเกี่ยวกับการจัดการการเข้าถึงแอปพลิเคชันของแขก ให้ดู[จัดการการเข้าถึงของแขกรับแขกด้วยการรีวิวการเข้าถึง Azure AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [เพิ่มผู้ใช้ที่](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)เป็นผู้ใช้ภายนอกลงในไดเรกทอรีของคุณในพอร์ทัล Azure : ในการเริ่มต้นใช้งานด่วนนี้ คุณจะเพิ่มผู้ใช้ที่เป็นผู้ใช้ภายนอกใหม่ในไดเรกทอรี Azure AD ผ่านพอร์ทัล Azure ส่งคําเชิญ และดูลักษณะของกระบวนการแลกใช้คําเชิญของผู้ใช้ภายนอก
1. [เพิ่มผู้ใช้ที่เป็นแขกด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): ในการเริ่มต้นใช้งานด่วนนี้ คุณจะใช้ New-AzureADMSInvitation สั่งเพื่อเพิ่มผู้ใช้ที่เป็นแขกหนึ่งรายลงในผู้เช่า Azure ของคุณ
1. เมื่อต้องการเรียนรู้วิธีการกําหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันขององค์กรใน Azure Active Directory (Azure AD) ไม่ว่าจะจากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell ให้ดู จัดการงานที่มอบหมาย[ของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)แอปใน Azure Active Directory 
1. Azure Active Directory (Azure AD) การร่วมมือกันแบบ B2B สามารถใช้งานร่วมกับแอปส่วนใหญ่ที่รวมกับ Azure AD ได้ ในบทความนี้ [เราจะแนะ](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)นําคําแนะนําในการกําหนดค่าแอป SaaS ยอดนิยมบางอย่างเพื่อใช้กับ Azure AD B2B
1. ในฐานะองค์กรที่ใช้ความสามารถในการร่วมมือกันระหว่าง Azure Active Directory (Azure AD) B2B เพื่อเชิญผู้ใช้ที่เป็นแขกจากองค์กรคู่ค้าไปยัง Azure AD ของคุณ ตอนนี้คุณสามารถให้ผู้ใช้ B2B เหล่านี้เข้าถึงแอปภายในองค์กรได้แล้ว แอปภายในองค์กรเหล่านี้สามารถใช้การรับรองความถูกต้องแบบ SAML หรือ การรับรองความถูกต้องแบบรวม Windows (IWA) กับการมอบสิทธิ์แบบมีข้อห้ามของ Kerberos (KCD) For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. เรียนรู้วิธีการให้[สิทธิ์การเข้าถึงบัญชีคู่ค้าที่มีการจัดการภายในเครื่องไปยังแหล่งข้อมูลระบบคลาวด์โดยใช้การร่วมมือกันระหว่าง Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)