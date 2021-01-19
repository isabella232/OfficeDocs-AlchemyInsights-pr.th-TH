---
title: แก้ไขปัญหาของผู้ใช้ที่เป็นผู้เยี่ยมชม
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901592"
---
# <a name="troubleshoot-guest-user-issues"></a>แก้ไขปัญหาของผู้ใช้ที่เป็นผู้เยี่ยมชม

1. สำหรับคำแนะนำเกี่ยวกับการจัดการการเข้าถึงแอปพลิเคชันของผู้เยี่ยมชมให้ดู[ที่จัดการการเข้าถึงของผู้เยี่ยมชมด้วย AZURE AD access รีวิว](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [เพิ่มผู้ใช้ที่เป็นผู้เยี่ยมชมลงในไดเรกทอรีของคุณในพอร์ทัล azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): ใน quickstart นี้คุณจะเพิ่มผู้ใช้ที่เป็นผู้เยี่ยมชมใหม่ลงในไดเรกทอรี AD azure ของคุณผ่านทางพอร์ทัล azure ส่งการเชิญและดูว่ากระบวนการแลกสิทธิ์การเชิญของผู้ใช้ที่เป็นผู้เยี่ยมชมมีลักษณะอย่างไร
1. [เพิ่มผู้ใช้ที่เป็นผู้เยี่ยมชมด้วย PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): ใน quickstart นี้คุณจะใช้คำสั่ง New-AzureADMSInvitation เพื่อเพิ่มผู้ใช้ที่เป็นผู้เยี่ยมชมหนึ่งรายไปยังผู้เช่า Azure ของคุณ
1. เมื่อต้องการเรียนรู้วิธีการกำหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันสำหรับองค์กรใน Azure Active Directory (Azure AD) จากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell ให้ดูที่[จัดการงานที่มอบหมายของผู้ใช้สำหรับแอปใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. การทำงานร่วมกันแบบ B2B ของ azure Active Directory (Azure AD) ทำงานร่วมกับแอปส่วนใหญ่ที่รวมเข้ากับ Azure AD ใน [บทความ](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)นี้เราจะเดินผ่านคำแนะนำสำหรับการกำหนดค่าแอป SaaS ที่ได้รับความนิยมบางส่วนสำหรับใช้กับ AZURE AD B2B
1. ในฐานะองค์กรที่ใช้ Azure Active Directory (Azure AD) ความสามารถในการทำงานร่วมกันแบบ B2B เพื่อเชิญผู้ใช้ที่เป็นผู้เยี่ยมชมจากองค์กรคู่ค้าไปยังโฆษณา Azure ของคุณตอนนี้คุณสามารถให้สิทธิ์ผู้ใช้ B2B เหล่านี้เข้าถึงแอปภายในองค์กรได้ แอปภายในองค์กรเหล่านี้สามารถใช้การรับรองความถูกต้องโดยใช้ SAML หรือการรับรองความถูกต้องของ Windows แบบรวม (IWA) ที่มีการมอบหมายของ Kerberos ที่จำกัด (KCD) สำหรับข้อมูลเพิ่มเติมให้ดู[ที่มอบสิทธิ์ผู้ใช้ B2B ในการเข้าถึง AZURE AD ไปยังแอปพลิเคชันภายในองค์กรของคุณ](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. เรียนรู้วิธีการให้ [สิทธิ์การเข้าถึงบัญชีผู้ใช้คู่ค้าที่มีการจัดการภายในกับทรัพยากร cloud โดยใช้ AZURE AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)การทำงานร่วมกัน