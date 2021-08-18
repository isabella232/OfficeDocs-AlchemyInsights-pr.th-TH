---
title: การจัดการกลุ่มการตั้งค่า
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: a988d792c51a81eac9aad3e8b2cd20fec9b2df51766f8919312e933a806e47ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114731"
---
# <a name="managing-external-settings"></a>การจัดการกลุ่มการตั้งค่า

**การประกาศ**

- [การเลิกใช้การสนับสนุนการลงชื่อเข้าใช้ WebView จาก Google ตั้งแต่วันที่ 4 มกราคม 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) ทดสอบว่าแอปของคุณได้รับผลกระทบจากแนวทางของ Google เกี่ยวกับการทดสอบความเข้ากันได้หรือไม่
- ตรวจสอบให้แน่ใจว่าได้ใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของผู้ใช้ทั่วไป

**จัดการบัตรเชิญการตั้งค่า**

ยืนยันว่าคุณได้กําหนด [การตั้งค่าการร่วมมือกันภายนอก](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) เพื่ออนุญาตให้บุคคลที่เหมาะสมสามารถส่งคําเชิญได้

**จัดการสิทธิ์การเข้าถึงของผู้ใช้ที่เป็นแขก**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การเข้าถึงของแขกในไดเรกทอรีผ่านพอร์ทัล Azure โดยการกําหนดค่าสิทธิ์การเข้าถึงของผู้ใช้ภายนอกบนหน้า การร่วมการตั้งค่าภายนอก [เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)นี้
2. หากคุณต้องการให้แขกของคุณเข้าถึงแอป เช่น Teamsหรือ SharePoint โปรดยืนยันว่าคุณได้กําหนดค่าแอปเหล่านั้นเพื่ออนุญาตการเข้าถึงของแขก เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า[Teams และ](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support)[SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**การกําหนดค่าคําเชิญ:**

- [เปิดใช้งานการร่วมมือกันภายนอกแบบ B2B และจัดการผู้ที่สามารถเชิญผู้ใช้ภายนอกได้](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [อนุญาตหรือบล็อกการเชิญไปยังผู้ใช้จากองค์กรที่ระบุ](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**การกําหนดค่าผู้ให้บริการข้อมูลเฉพาะตัวที่อนุญาต:**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [การติดต่อกับภายนอกโดยตรง](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ส่งการรับรองความถูกต้องรหัสผ่านแบบใช้อีเมลแบบใช้เวลาเดียว](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
