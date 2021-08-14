---
title: Privileged Identity Managementบทบาท
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973248"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**สิทธิ์จะไม่ถูกมอบหลังจากเปิดใช้งานบทบาท**

เมื่อคุณเปิดใช้งานบทบาทใน Azure AD Privileged Identity Management (PIM) การเปิดใช้งานอาจไม่เผยแพร่ไปยังพอร์ทัลทั้งหมดที่ต้องใช้บทบาทที่มีสิทธิ์ทันที แม้ว่าการเปลี่ยนแปลงจะเผยแพร่ไปยังบางครั้ง การแคชเว็บในพอร์ทัลอาจส่งผลให้การเปลี่ยนแปลงไม่มีผลในทันที

ถ้าการเปิดใช้งานของคุณล่าช้า ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ลงชื่อออกจากพอร์ทัล Azure แล้วลงชื่อเข้าใช้อีกครั้ง เมื่อคุณเปิดใช้งานบทบาท Azure AD หรือบทบาททรัพยากร Azure คุณจะเห็นขั้นตอนการเปิดใช้งานของคุณ เมื่อขั้นตอนทั้งหมดเสร็จสมบูรณ์ คุณจะเห็นลิงก์ 'ลงชื่อออก' คุณสามารถใช้ลิงก์นี้เพื่อลงชื่อออก การแก้ไขปัญหานี้จะแก้ไขกรณีส่วนใหญ่เพื่อหน่วงเวลาการเปิดใช้งาน
2. ใน PIM ให้ตรวจสอบว่าคุณเป็นสมาชิกของบทบาท
3. ถ้าคุณเปิดใช้งานบทบาทผู้ดูแลระบบExchange ตรวจสอบให้แน่ใจว่าคุณได้ลงชื่อออกและลงชื่อเข้าใช้อีกครั้ง ถ้าปัญหายังคงอยู่ ให้เปิดตั๋วการสนับสนุนและแจ้งปัญหานี้เป็นปัญหา ถ้าคุณใช้บทบาทผู้ดูแลระบบ Exchangeของคุณในการเข้าถึงศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย ให้ดูขั้นตอนถัดไป
4. ถ้าคุณเปิดใช้งานบทบาทเพื่อเข้าถึงศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย หรือถ้าคุณเปิดใช้งานบทบาทผู้ดูแลระบบ SharePoint คุณจะพบความล่าช้าในการเปิดใช้งานบางอย่างตั้งแต่สองสามนาทีถึงสองสามชั่วโมง นี่เป็นปัญหาที่ทราบแล้วและเราจะพยายามแก้ไขทีมเหล่านี้ให้เร็วที่สุด

สำหรับข้อมูลเพิ่มเติม ให้ดู:

- [เปิดใช้งานบทบาท Azure AD ของฉันใน PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [เปิดใช้งานบทบาททรัพยากร Azure ของฉันใน PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**สิทธิ์จะไม่ถูกเอาออกหลังจากปิดใช้งานบทบาทหรือการเปิดใช้งานบทบาทหมดอายุ**

เมื่อคุณปิดใช้งานบทบาทใน Azure AD Privileged Identity Managementหรือเมื่อระยะเวลาการเปิดใช้งานบทบาทหมดอายุ อาจมีความล่าช้าที่คุณยังคงเข้าถึงได้

ถ้าการปิดใช้งานของคุณล่าช้า ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ถ้าคุณปิดใช้งานบทบาทผู้ดูแลระบบ Exchange หรือระยะเวลาการเปิดใช้งานบทบาทหมดอายุ และคุณจะสังเกตเห็นความล่าช้าอย่างมากก่อนที่สิทธิ์จะถูกเอาออก ให้เปิดตั๋วการสนับสนุน และบอกวิศวกรฝ่ายสนับสนุนของคุณเพื่อช่วยคุณจัดตั๋วกับทีมการจัดการการเข้าถึง (PAM) ที่ได้รับสิทธิ์ภายใน Office เกี่ยวกับปัญหานี้
2. ถ้าระยะเวลาการเปิดใช้งานหมดอายุแล้ว แต่คุณยังคงเปิดเซสชันของเบราว์เซอร์อยู่ ให้ปิดเบราว์เซอร์ของคุณ คุณสามารถใช้บทบาทต่อไปได้จนกว่าคุณจะปิดเซสชันนั้น นี่เป็นปัญหาที่ทราบแล้ว และเราดูการแก้ไขที่อาจเกิดขึ้นเพื่อยกเลิกแต่ละเซสชันเมื่อการเปิดใช้งานหมดอายุแล้ว

หากความล่าช้าของคุณแตกต่างจากสองสถานการณ์นี้ โปรดเปิดตั๋วการสนับสนุน
