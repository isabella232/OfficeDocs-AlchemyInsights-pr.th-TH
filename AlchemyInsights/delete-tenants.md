---
title: ลบผู้เช่า
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564878"
---
# <a name="delete-tenant"></a>ลบผู้เช่า

เมื่อต้องการลบโฆษณา Azure ให้ตรวจสอบให้แน่ใจว่า:
- คุณเป็นผู้ดูแลระบบส่วนกลางบนไดเรกทอรี
- คุณไม่ได้ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ที่มีไดเรกทอรีเริ่มต้นเช่น contoso.onmicrosoft.com ในบัญชีผู้ใช้ที่ลงชื่อเข้าใช้เช่น admin@contoso.onmicrosoft.com
- เอาแอปพลิเคชันที่ใช้งานอยู่ในไดเรกทอรีออกก่อนการลบ เมื่อต้องการเอาแอปพลิเคชันที่ใช้งานอยู่ออกให้นำทางไปยังการลงทะเบียนแอปและเอาแอปพลิเคชัน
- ไม่มีการสมัครใช้งานที่ใช้งานอยู่สำหรับบริการ Microsoft Online ใดๆเช่น Microsoft Azure, Office ๓๖๕หรือ Azure AD Premium ที่เกี่ยวข้องกับไดเรกทอรี โอนการสมัครใช้งานของคุณหรือยกเลิกการสมัครใช้งานที่ใช้งานได้ผ่านทางการสนับสนุนและการเรียกเก็บเงินของ Azure เรียนรู้เพิ่มเติมเกี่ยวกับวิธีการยกเลิกการสมัครใช้งาน Office ๓๖๕และ Azure สำหรับคำแนะนำเกี่ยวกับการเชื่อมโยงหรือการเพิ่มการสมัครใช้งานที่มีอยู่ให้กับผู้เช่าให้ดูที่[เชื่อมโยงหรือเพิ่มการสมัครใช้งาน azure ไปยังผู้เช่า AZURE AD ของคุณ](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- ไม่มีสิทธิ์การใช้งานที่ใช้งานอยู่ เมื่อต้องการเอาสิทธิ์การใช้งานออกให้ดู[วิธีการเอาการสมัครใช้งานออกเพื่อเอาสิทธิ์การใช้งานออก](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- ไม่มีผู้ใช้ที่ใช้งานอยู่อื่นในไดเรกทอรีนอกเหนือจากตัวคุณเองเป็นผู้ดูแลระบบส่วนกลางเมื่อพยายามลบโฆษณา Azure เอาผู้ใช้ที่ใช้งานอยู่และการอ้างอิงใดๆบนชื่อโดเมนแบบกำหนดเองในผู้เช่าจะต้องถูกเอาออกเช่นผู้ใช้ที่สร้างด้วย admin@contoso.com

สำหรับขั้นตอนรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการ:
- ลบ "Azure Active Directory" หรือ "การสมัครใช้งาน" ให้ดู[ลบไดเรกทอรีที่ใช้งานอยู่ของ azure](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- การเอาแอปพลิเคชันในไดเรกทอรีออกให้ดูที่การ [เอาแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)ออก 
