---
title: การจัดการการตั้งค่าภายนอก
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
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294431"
---
# <a name="managing-external-settings"></a>การจัดการการตั้งค่าภายนอก

**การประกาศ**

- [การเลิกใช้การสนับสนุนการลงชื่อเข้าใช้ WebView จาก Google ตั้งแต่วันที่ 4 มกราคม 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) ทดสอบว่าแอปของคุณได้รับผลกระทบจากตามแนวทางของ Google เกี่ยวกับการทดสอบความเข้ากันได้หรือไม่
- ตรวจสอบให้แน่ใจว่าได้ใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของผู้ใช้ทั่วไป

**จัดการการตั้งค่าการเชิญ**

ยืนยันว่าคุณได้กําหนด [ค่าการตั้งค่าการร่วมมือกัน](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) ภายนอกเพื่อให้บุคคลที่เหมาะสมสามารถส่งคําเชิญได้

**จัดการสิทธิ์การเข้าถึงของผู้ใช้ที่เป็นแขก**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การเข้าถึงของแขกในไดเรกทอรีผ่านพอร์ทัล Azure โดยการกําหนดค่าสิทธิ์การเข้าถึงของผู้ใช้ภายนอกบนหน้าการตั้งค่าการร่วมมือกันภายนอก [เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)นี้
2. หากคุณต้องการให้แขกของคุณเข้าถึงแอป เช่น Teams หรือ SharePoint ให้ยืนยันว่าคุณได้กําหนดค่าแอปเหล่านั้นให้อนุญาตการเข้าถึงของแขกแล้ว เรียนรู้เพิ่มเติมเกี่ยวกับการตั้งค่า[Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [และ SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**การกําหนดค่าคําเชิญ:**

- [เปิดใช้งานการร่วมมือกันภายนอก B2B และจัดการผู้ที่สามารถเชิญผู้ใช้ภายนอกได้](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [อนุญาตหรือบล็อกคําเชิญให้ผู้ใช้จากองค์กรที่ระบุ](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**การกําหนดค่าผู้ให้บริการข้อมูลเฉพาะตัวที่อนุญาต:**

- [การติดต่อกับภายนอกของ Google](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [การติดต่อกับภายนอกโดยตรง](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ส่งอีเมลการรับรองความถูกต้องรหัสผ่านแบบใช้เวลาเดียว](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
