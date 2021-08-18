---
title: สร้างผู้ใช้
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323305"
---
# <a name="create-user"></a>สร้างผู้ใช้

**ประกาศ:**

- [การเลิกใช้การสนับสนุนการลงชื่อเข้าใช้ WebView จาก Google ตั้งแต่วันที่ 4 มกราคม 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) ทดสอบว่าแอปของคุณอาจได้รับผลกระทบจากแนวทาง [ของ Google เกี่ยวกับ](https://go.microsoft.com/fwlink/?linkid=2157323) การทดสอบความเข้ากันได้หรือไม่
- ตรวจสอบให้แน่ใจว่าคุณใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของลูกค้า For more information, [see Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**ฉันไม่สามารถสร้างผู้ใช้ใหม่ในไดเรกทอรี Azure AD ของฉัน**

1. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างผู้ใช้มาตรฐานใหม่ เฉพาะผู้ดูแลระบบส่วนกลางหรือบทบาทผู้ดูแลระบบผู้ใช้ใน Azure Active Directory (AD) เท่านั้นที่สามารถสร้างผู้ใช้มาตรฐานใหม่ได้ ถ้าคุณไม่ได้อยู่ในบทบาทใดบทบาทหนึ่ง ให้ขอให้ผู้ดูแลระบบเพิ่มคุณลงในบทบาทเหล่านี้ หรือสร้างบัญชีผู้ใช้ใหม่ให้คุณ
1. ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ได้รับการยืนยันใน Azure AD ของคุณ ถ้าคุณไม่มีชื่อโดเมนแบบปรับแต่งเองที่ตรวจสอบแล้วใน Azure AD คุณสามารถใช้โดเมนเริ่มต้น Azure AD ของคุณ ซึ่งลงท้ายด้วย *.onmicrosoft.com
1. ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ไม่ได้ติดต่อกับภายนอก Azure AD จาก AD ภายในองค์กรของคุณ ผู้ใช้ไม่สามารถเพิ่มในระบบคลาวด์ด้วยชื่อโดเมนที่ติดต่อกับภายนอกจากภายในองค์กรได้
1. ตรวจสอบให้แน่ใจว่าไม่มีผู้ใช้หรือที่ติดต่ออื่นมีชื่อผู้ใช้ที่คุณต้องการกําหนดให้กับผู้ใช้ใหม่แล้ว ชื่อผู้ใช้ต้องไม่ซ.ก. ใน Azure AD
1. ดู [บทบาทและผู้ดูแลระบบ Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ของ Azure AD
1. ดู [ชื่อโดเมนของ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD ของคุณ
1. ตรวจทาน [บันทึก](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) การตรวจสอบเพื่อดูข้อมูลโดยละเอียดเพิ่มเติมเกี่ยวกับผู้ใช้ที่สร้างหรือลบเมื่อเร็วๆ นี้ เช่น ผู้ที่เริ่มการแอคชันและเมื่อใด
1. For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [บทบาทผู้ดูแลระบบ Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): สิทธิ์บทบาทผู้ดูแลระบบในAzure Active Directory
1. You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
