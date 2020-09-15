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
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664189"
---
# <a name="about-identity-in-yammer"></a>เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer

ขอแนะนำว่าเครือข่ายทั้งหมดจะทำตามขั้นตอนต่อไปนี้เพื่อหลีกเลี่ยงปัญหาที่เกี่ยวข้องกับข้อมูลเฉพาะตัว:

1. บังคับใช้ข้อมูลประจำตัวของ Office ๓๖๕หลังจากการเตรียมใช้งานบัญชีผู้ใช้ Microsoft ๓๖๕สำหรับผู้ใช้ใน Azure AD เพื่อให้แน่ใจว่าผู้ใช้ทั้งหมดลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ Microsoft ๓๖๕หลักของพวกเขา สำหรับข้อมูลเพิ่มเติมให้ดูที่[บังคับใช้ข้อมูลประจำตัวของ Office ๓๖๕สำหรับผู้ใช้ Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. รวมเครือข่าย Yammer หลายเครือข่าย การกำหนดค่า Yammer ดั้งเดิมอนุญาตให้เครือข่าย Yammer หลายเครือข่ายเชื่อมต่อกับผู้เช่าหนึ่งราย สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[โยกย้ายเครือข่ายรวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. อีกวิธีหนึ่งคือบังคับให้มีสิทธิ์การใช้งานสำหรับ Yammer เพื่อบล็อกผู้ใช้จาก Yammer ถ้าพวกเขาไม่มีสิทธิ์การใช้งาน สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. สุดท้ายให้ตรวจสอบรายชื่อผู้ใช้สำหรับเครือข่าย Yammer รุ่นเก่าและหยุดผู้ใช้แบบดั้งเดิม ขอแนะนำให้คุณระงับ (ปิดใช้งาน) ผู้ใช้แทนที่จะลบออกเนื่องจากการลบจะไม่สามารถย้อนกลับได้ สำหรับข้อมูลเพิ่มเติมให้ดูการ[ตรวจสอบผู้ใช้ Yammer ในเครือข่ายที่เชื่อมต่อกับ Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)และ[เอาผู้ใช้ออก](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

ด้วยการกำหนดค่า Yammer โดยใช้ขั้นตอนเหล่านี้คุณจะพร้อมที่จะกำหนดค่าเครือข่าย Yammer ของคุณสำหรับโหมด Native ของ Microsoft ๓๖๕ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การกำหนดค่าเครือข่าย Yammer ของคุณสำหรับโหมด Native สำหรับ Microsoft ๓๖๕](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)