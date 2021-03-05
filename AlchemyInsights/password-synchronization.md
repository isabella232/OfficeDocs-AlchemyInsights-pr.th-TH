---
title: การซิงโครไนซ์รหัสผ่าน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483086"
---
# <a name="password-synchronization"></a>การซิงโครไนซ์รหัสผ่าน

**การซิงโครไนซ์แฮชของรหัสผ่านไม่สมบูรณ์**

ปัญหาทั่วไปที่ลูกค้าพบเมื่อการซิงโครไนซ์แฮชของรหัสผ่านใช้งานไม่ได้:

- บัญชี Active Directory ที่ใช้โดย Azure AD Connect เพื่อสื่อสารกับ Active Directory ภายในองค์กรจะไม่ได้รับอนุญาตให้ **Replicate Directory Changes** และ **Replicate Directory Changes** All ซึ่งต้องใช้ในการซิงโครไนซ์รหัสผ่าน คุณจึงต้องแก้ไขปัญหานี้โดยให้สิทธิ์เหล่านี้กับบัญชี Active Directory
- การซิงโครไนซ์แฮชรหัสผ่านจะถูกปิดใช้งานหลังจากผู้ดูแลระบบเปลี่ยนวิธี Sign-In ผู้ใช้จากการซิงโครไนซ์รหัสผ่านเป็นตัวเลือกอื่น เช่น การติดต่อกับภายนอกด้วย **AD FS** ในตัวช่วยสร้าง Azure AD Connect - คุณสามารถแก้ไขปัญหานี้ได้โดยการเปิดใช้งานฟีเจอร์การซิงโครไนซ์แฮชของรหัสผ่านอีกครั้งในตัวช่วยสร้าง Azure AD Connect
- ปัญหาการเชื่อมต่อกับ Active Directory ภายในองค์กร ตัวอย่างเช่น บางตัวควบคุมโดเมนไม่สามารถเข้าถึงได้โดย Azure AD Connect หรือพอร์ตที่ต้องมีถูก[](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)บล็อกโดยไฟร์วอลล์ คุณจึงต้องแก้ไขปัญหานี้โดยการตรวจสอบให้แน่ใจว่าการเชื่อมต่อระหว่างเซิร์ฟเวอร์ Azure AD Connect และ Active Directory ภายในองค์กรสามารถใช้งานได้อย่างถูกต้อง
- เซิร์ฟเวอร์ Azure AD Connect ที่อยู่ในโหมดการจัดเตรียมอยู่ในขณะนี้ ซึ่งจะส่งผลให้เซิร์ฟเวอร์ไม่สามารถไปที่ Hashes ของรหัสผ่านได้ - เมื่อต้องการแก้ไขปัญหา ให้ปฏิบัติตามขั้นตอนที่อธิบายไว้ในส่วนแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านด้วย [การซิงค์ Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)ไม่มีการซิงโครไนซ์รหัสผ่าน

**การซิงโครไนซ์แฮชของรหัสผ่านไม่ใช้งานกับผู้ใช้บางรายของฉัน**

1. ถ้าคุณสังเกตเห็นว่าแฮชของรหัสผ่านไม่ซิงค์กับผู้ใช้ ให้ใช้งาน **แก้ไขปัญหา** ใน Azure AD Connect เพื่อตรวจสอบและแก้ไขปัญหา ให้ดการงานต่อไปนี้

    a. [เรียกใช้งานการแก้ไขปัญหาในตัวช่วยสร้าง](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [ใช้ cmdlet การแก้ไขปัญหาเพื่อตรวจสอบปัญหาการซิงค์แฮชรหัสผ่านในการใช้งานเฉพาะ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. วัตถุผู้ใช้ Active Directory ภายในองค์กรถูกเปิดใช้งานไว้ **เพื่อให้ผู้ใช้ต้องเปลี่ยนรหัสผ่านที่ตัวเลือกการเข้าสู่ระบบ** ถัดไป เมื่อเปิดใช้งานตัวเลือกนี้ ผู้ใช้จะถูกมอบหมายรหัสผ่านชั่วคราวและจะได้รับพร้อมท์ให้เปลี่ยนรหัสผ่านบนการเข้าสู่ระบบครั้งถัดไป Azure AD Connect ไม่ซิงโครไนซ์รหัสผ่านชั่วคราวกับ Azure AD

เมื่อต้องการแก้ไขปัญหาข้างต้น ให้ปฏิบัติอย่างใดอย่างหนึ่งต่อไปนี้:

- ขอให้ผู้ใช้ลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กร (ตัวอย่างเช่น เดสก์ท็อป Windows) และเปลี่ยนรหัสผ่าน รหัสผ่านใหม่จะถูกซิงโครไนซ์กับ Azure AD
- ให้ผู้ดูแลระบบอัปเดตรหัสผ่านของผู้ใช้โดยไม่เปิดใช้งานตัวเลือก ที่ผู้ใช้ต้องเปลี่ยนรหัสผ่าน **ในการเข้าสู่ระบบ** ครั้งถัดไป และแชร์รหัสผ่านใหม่กับผู้ใช้

3. วัตถุผู้ใช้ Active Directory ภายในองค์กรไม่ได้ถูก **กําหนดค่าอย่างถูกต้องในการ** ซิงโครไนซ์วัตถุหรือการซิงโครไนซ์รหัสผ่าน เมื่อต้องการแก้ไขปัญหานี้ ให้ปฏิบัติตามขั้นตอนที่อธิบายไว้ในการซิงโครไนซ์แฮช[ของรหัสผ่านการแก้ไขปัญหาด้วยการซิงค์ Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







