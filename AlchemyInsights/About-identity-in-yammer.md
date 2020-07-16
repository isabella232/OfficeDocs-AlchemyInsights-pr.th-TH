---
title: เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148425"
---
# <a name="about-identity-in-yammer"></a>เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer

ขอแนะนําให้เครือข่ายทั้งหมดทําตามขั้นตอนต่อไปนี้เพื่อหลีกเลี่ยงปัญหาที่เกี่ยวข้องกับข้อมูลประจําตัว:

1. บังคับใช้ข้อมูลประจําตัวของ Office 365 หลังจากเตรียมใช้งานบัญชี Microsoft 365 สําหรับผู้ใช้ใน Azure AD เพื่อให้แน่ใจว่า ผู้ใช้ทุกคนเข้าสู่ระบบ โดยใช้บัญชี Microsoft 365 หลักของพวกเขา สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การบังคับใช้ข้อมูลประจําตัวของ Office 365 สําหรับผู้ใช้ Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. รวมเครือข่าย Yammer หลายเครือข่าย การกําหนดค่า Yammer แบบดั้งเดิมอนุญาตให้หลายเครือข่าย Yammer สามารถเชื่อมต่อกับผู้เช่าหนึ่งราย สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การโยกย้ายเครือข่าย - รวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. หรือบังคับให้มีการอนุญาตให้ใช้สิทธิ์สําหรับ Yammer เพื่อบล็อกผู้ใช้จาก Yammer ถ้าผู้ใช้ไม่มีสิทธิ์การใช้งาน สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. สุดท้าย ตรวจสอบรายการผู้ใช้สําหรับเครือข่าย Yammer รุ่นเก่า และระงับผู้ใช้แบบดั้งเดิม ขอแนะนําให้คุณระงับผู้ใช้ (ปิดใช้งาน) แทนการลบเนื่องจากการลบกลับไม่ได้ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตรวจสอบผู้ใช้ Yammer ในเครือข่ายที่เชื่อมต่อกับ Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)และ[นําผู้ใช้ออก](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

ด้วยการกําหนดค่า Yammer โดยใช้ขั้นตอนเหล่านี้ คุณจะพร้อมที่จะกําหนดค่าเครือข่าย Yammer ของคุณสําหรับโหมดดั้งเดิมสําหรับ Microsoft 365 สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การตั้งค่าคอนฟิกเครือข่าย Yammer ของคุณสําหรับโหมดเนทิฟสําหรับ Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)