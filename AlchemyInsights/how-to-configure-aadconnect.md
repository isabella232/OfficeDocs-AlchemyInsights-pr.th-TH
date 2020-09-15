---
title: ๖๔๖วิธีการกำหนดค่า AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704508"
---
# <a name="configure-sync-features"></a>กำหนดค่าฟีเจอร์การซิงค์

Azure AD Connect มีฟีเจอร์หลายอย่างที่จะเปิดใช้งานตามค่าเริ่มต้นหรือคุณสามารถเปิดใช้งานในภายหลังได้ ฟีเจอร์บางอย่างจำเป็นต้องมีการกำหนดค่าเพิ่มเติมในสภาพแวดล้อมที่เฉพาะเจาะจง

- การ[กรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)จำกัดวัตถุจะถูกซิงโครไนซ์กับ Azure AD ตามค่าเริ่มต้นผู้ใช้ที่ติดต่อกลุ่มและบัญชีผู้ใช้ Windows 10 ทั้งหมดจะถูกซิงโครไนซ์ คุณสามารถรวมหรือแยกวัตถุได้โดยยึดตามโดเมน Ou หรือแอตทริบิวต์อื่นๆ

- การ[ซิงโครไนซ์แฮชของรหัสผ่านซิ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)งโครไนซ์แฮชของรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรไปยัง Azure AD การทำเช่นนี้จะช่วยให้การจัดการรหัสผ่านในตำแหน่งที่ตั้งเดียวแต่ใช้รหัสผ่านเดียวกันในสภาพแวดล้อมทั้งภายในองค์กรและระบบคลาวด์ เนื่องจาก Active Directory เป็นแหล่งข้อมูลที่มีสิทธิ์คุณสามารถใช้นโยบายรหัสผ่านของคุณเองได้

- การ[ตั้งค่ารหัสผ่านแบบบริการตนเอง (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)อนุญาตให้ผู้ใช้รีเซ็ตรหัสผ่านของตนเองในระบบคลาวด์ได้ในขณะที่ยังคงใช้นโยบายรหัสผ่านภายในองค์กรของคุณ

- [อุปกรณ์ writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ช่วยให้อุปกรณ์ที่ลงทะเบียนใน Azure AD จะถูกเขียนกลับไปยัง active directory ภายในองค์กรเพื่อให้สามารถใช้สำหรับการเข้าถึงแบบมีเงื่อนไขได้

- การ[ป้องกันการลบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)โดยไม่ตั้งใจจะถูกเปิดใช้งานตามค่าเริ่มต้นเพื่อช่วยป้องกันไม่ให้มีการลบวัตถุพร้อมกันจำนวนมากเกินไป (วัตถุมากกว่า๕๐๐ต่อการซิงโครไนซ์) คุณสามารถเปลี่ยนการตั้งค่านี้เพื่อตอบสนองความต้องการขององค์กรของคุณ

- การ[อัปเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)จะถูกเปิดใช้งานตามค่าเริ่มต้นสำหรับการติดตั้งแบบด่วนและช่วยให้แน่ใจว่าเวอร์ชันของ Azure AD Connect ของคุณเป็นปัจจุบันเสมอ
