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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993912"
---
# <a name="delete-tenant"></a>ลบผู้เช่า

เมื่อต้องการลบ Azure AD ตรวจสอบให้แน่ใจว่า:
- คุณเป็นผู้ดูแลระบบส่วนกลางในไดเรกทอรี
- คุณไม่ได้ลงชื่อเข้าใช้ด้วยบัญชีที่มีไดเรกทอรีเริ่มต้น เช่น contoso.onmicrosoft.com บัญชีที่ลงชื่อเข้าใช้ เช่น บัญชี admin@contoso.onmicrosoft.com
- เอาแอปพลิเคชันที่ใช้งานอยู่ใดๆ ในไดเรกทอรีออกก่อนที่จะลบ เมื่อต้องการนําแอปพลิเคชันที่ใช้งานอยู่ออก ให้นําทางไปยัง การลงทะเบียนแอป แล้วนําแอปพลิเคชันที่มีอยู่ออก
- ไม่มีการสมัครใช้งานที่ใช้งานอยู่ของ Microsoft Online Services เช่น Microsoft Azure, Office 365 หรือ Azure AD Premium ที่เชื่อมโยงกับไดเรกทอรี ถ่ายโอนการสมัครใช้งานของคุณหรือการยกเลิกการสมัครใช้งานที่ใช้งานแบบเร่งรีบผ่านการสนับสนุนและการเรียกเก็บเงินของ Azure เรียนรู้เพิ่มเติมเกี่ยวกับ วิธีการยกเลิกOffice 365การสมัครใช้งาน Azure สําหรับแนวทางเกี่ยวกับการเชื่อมโยงหรือการเพิ่มการสมัครใช้งานที่มีอยู่ไปยังผู้เช่า ให้ดู เชื่อมโยง [หรือเพิ่มการสมัครใช้งาน Azure ไปยังผู้เช่า Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)ของคุณ
- ไม่มีสิทธิ์การใช้งานที่ใช้งานอยู่ To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- ไม่มีผู้ใช้ที่ใช้งานอยู่รายอื่นๆ ในไดเรกทอรีนอกเหนือจากตัวคุณเองในฐานะผู้ดูแลระบบส่วนกลางเมื่อพยายามลบ Azure AD เอาผู้ใช้อื่นที่ใช้งานอยู่ออก และการขึ้นต่อกันใดๆ บนชื่อโดเมนแบบ admin@contoso.com ในผู้เช่า

ดูขั้นตอนโดยละเอียดเพิ่มเติมเกี่ยวกับวิธีการ:
- ลบ "Azure Active Directory" หรือ "การสมัครใช้งาน"[ให้ดู Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- การเอาแอปพลิเคชันในไดเรกทอรีออก [ให้ดู การเอาแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)ออก 
