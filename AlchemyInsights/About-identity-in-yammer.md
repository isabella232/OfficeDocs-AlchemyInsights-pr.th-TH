---
title: เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918956"
---
# <a name="about-identity-in-yammer"></a>เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer

เราแนะนนะให้ทุกเครือข่ายปฏิบัติตามขั้นตอนต่อไปนี้เพื่อหลีกเลี่ยงปัญหาที่เกี่ยวข้องกับข้อมูลเฉพาะตัว

1. บังคับใช้Office 365ของผู้ใช้หลังจากเตรียมใช้งานMicrosoft 365บัญชีหลักของผู้ใช้ใน Azure AD เพื่อให้แน่ใจว่าผู้ใช้ทั้งหมดลงชื่อเข้าใช้โดยใช้บัญชีหลักMicrosoft 365ของพวกเขา For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. รวมเครือข่ายYammerหลายเครือข่าย การกําหนดYammerดั้งเดิมจะอนุญาตให้Yammerหลายเครือข่ายสามารถเชื่อมต่อกับผู้เช่าเดียวได้ For more info, see [Network migration - Consolidated multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. หรือ บังคับใช้การให้สิทธิ์การใช้งานYammerบล็อกผู้ใช้Yammerหรือไม่ก็ได้ ถ้าพวกเขาไม่มีสิทธิ์การใช้งาน For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. สุดท้าย ตรวจสอบรายชื่อผู้ใช้ของเครือข่ายเวอร์ชันYammerและระงับผู้ใช้แบบดั้งเดิม ขอแนะนให้คุณระงับ (ปิดใช้งาน) ผู้ใช้แทนการลบ เนื่องจากการลบไม่สามารถย้อนกลับได้ For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and Remove [users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

เมื่อกําหนดYammerการตั้งค่าโดยใช้ขั้นตอนเหล่านี้ คุณก็พร้อมที่จะกําหนดค่าเครือข่าย Yammer ของคุณMicrosoft 365โหมดดั้งเดิม ดูข้อมูลเพิ่มเติมได้ที่ กําหนดค่า[เครือข่าย Yammerของคุณในโหมดดั้งเดิม Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)