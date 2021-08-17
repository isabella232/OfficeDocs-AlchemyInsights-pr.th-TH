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
ms.openlocfilehash: c4059364cd8aba920dba833c88a69413bad95a2c3b895599d9f6895b50ff73d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079649"
---
# <a name="deploy-ad-fs"></a>ปรับใช้ AD FS

การปรับใช้ Active Directory Federation Services (AD FS) ใช้โครงสร้างพื้นฐานภายในองค์กรของคุณเพื่อรับรองความถูกต้องของผู้ใช้Office 365บริการของคุณ ด้วยการลงชื่อเข้าใช้แบบติดต่อกับภายนอก คุณสามารถให้ผู้ใช้ลงชื่อเข้าใช้แอปพลิเคชัน Office 365 Services และ Software as a Service (SAAS) ที่รวมกับ Azure Active Directory (Azure AD) ได้ การลงชื่อเข้าใช้แบบติดต่อกับภายนอกรับรองความถูกต้องของผู้ใช้กับ Active Directory ภายในองค์กรของคุณผ่านทาง AD FS นอกจากนี้ ในขณะที่อยู่บนเครือข่ายขององค์กร ผู้ใช้ไม่ตําเป็นต้องใส่รหัสผ่านของพวกเขาอีกครั้ง

โปรแกรม[ช่วยแนะนํา](https://go.microsoft.com/fwlink/?linkid=2071178)การปรับใช้ AD FS มีแนวทางทีละขั้นตอนเกี่ยวกับการปรับใช้โครงสร้างพื้นฐาน AD FS ในสถานที่ที่รับรองความถูกต้องของผู้ใช้สําหรับMicrosoft 365 Office 365และบริการต่างๆ ด้วยคู่มือนี้ องค์กรของคุณสามารถรีวิวคอมโพเนนต์และข้อจําเป็นของ AD FS รับและติดตั้งใบรับรอง SSL ที่จําเป็นในการปรับใช้ และติดตั้งพร็อกซีเซิร์ฟเวอร์แอปพลิเคชันบนเว็บที่จําเป็น
