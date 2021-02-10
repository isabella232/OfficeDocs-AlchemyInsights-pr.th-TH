---
title: ปรับใช้ AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177714"
---
# <a name="deploy-ad-fs"></a>ปรับใช้ AD FS

การปรับใช้ Active Directory Federation Services (AD FS) จะใช้โครงสร้างพื้นฐานภายในองค์กรของคุณเพื่อรับรองความถูกต้องของผู้ใช้บริการ Office 365 ด้วยการลงชื่อเข้าใช้แบบติดต่อกับภายนอก คุณสามารถให้ผู้ใช้ลงชื่อเข้าใช้บริการ Office 365 และแอปพลิเคชันซอฟต์แวร์เป็นบริการ (SAAS) ที่รวมกับ Azure Active Directory (Azure AD) ได้ การลงชื่อเข้าใช้แบบติดต่อกับภายนอกจะรับรองความถูกต้องของผู้ใช้กับ Active Directory ภายในองค์กรของคุณผ่าน AD FS นอกจากนี้ ในขณะที่อยู่บนเครือข่ายขององค์กร ผู้ใช้จะไม่ต้องใส่รหัสผ่านอีกครั้ง

โปรแกรม [ช่วยแนะนํา](https://go.microsoft.com/fwlink/?linkid=2071178) การปรับใช้ AD FS จะแนะนําทีละขั้นตอนเกี่ยวกับการปรับใช้โครงสร้างพื้นฐาน AD FS ภายในองค์กรที่รับรองความถูกต้องของผู้ใช้สําหรับบริการ Microsoft 365 และ Office 365 ด้วยคู่มือนี้ องค์กรของคุณสามารถตรวจทานคอมโพเนนต์และความต้องการ AD FS รับและติดตั้งใบรับรอง SSL ที่จําเป็นในการปรับใช้ และติดตั้งพร็อกซีเซิร์ฟเวอร์แอปพลิเคชันบนเว็บที่จําเป็น
