---
title: 646 วิธีกําหนดค่า AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963662"
---
# <a name="configure-sync-features"></a>กําหนดค่าฟีเจอร์การซิงค์

Azure AD เชื่อมต่อมีฟีเจอร์หลายอย่างที่เปิดใช้งานตามค่าเริ่มต้น หรือคุณสามารถเปิดใช้งานในภายหลังได้ ฟีเจอร์บางอย่างต้องการการกําหนดค่าเพิ่มเติมในสภาพแวดล้อมที่เฉพาะเจาะจง

- [การกรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) จะจํากัดวัตถุที่ซิงโครไนซ์กับ Azure AD ตามค่าเริ่มต้น ผู้ใช้ ที่ติดต่อ กลุ่ม และบัญชีWindows 10ทั้งหมดจะถูกซิงโครไนซ์ คุณสามารถรวมหรือแยกวัตถุที่ยึดตามโดเมน OUs หรือแอตทริบิวต์อื่นๆ

- [การซิงโครไนซ์แฮช](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) ของรหัสผ่านจะซิงโครไนซ์แฮชรหัสผ่านจาก Active Directory ภายในองค์กรกับ Azure AD ซึ่งช่วยให้สามารถจัดการรหัสผ่านได้ภายในที่เดียว แต่สามารถใช้รหัสผ่านเดียวกันได้ทั้งในสภาพแวดล้อมภายในองค์กรและระบบคลาวด์ เนื่องจาก Active Directory เป็นแหล่งข้อมูลที่ใช้ทางการ คุณสามารถใช้นโยบายรหัสผ่านของคุณเองได้

- [การตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ช่วยให้ผู้ใช้สามารถรีเซ็ตรหัสผ่านของตนเองในระบบคลาวด์ในขณะที่ยังคงใช้นโยบายรหัสผ่านภายในองค์กรของคุณ

- [การเขียนกลับ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ของอุปกรณ์อนุญาตให้อุปกรณ์ที่ลงทะเบียนใน Azure AD สามารถเขียนกลับไปยัง Active Directory ภายในองค์กรเพื่อให้สามารถใช้เพื่อเข้าถึงตามเงื่อนไขได้

- [การป้องกันการลบโดยไม่ตั้งใจ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) จะถูกเปิดใช้งานตามค่าเริ่มต้นเพื่อช่วยป้องกันไม่ให้มีการลบวัตถุพร้อมกันมากเกินไป (วัตถุมากกว่า 500 รายการต่อหนึ่งการซิงโครไนซ์) คุณสามารถเปลี่ยนการตั้งค่านี้เพื่อให้ตรงตามความต้องการขององค์กรของคุณ

- [การอัปเกรด](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)อัตโนมัติจะถูกเปิดใช้งานตามค่าเริ่มต้นเพื่อการติดตั้งแบบด่วน และช่วยให้แน่ใจว่าเวอร์ชันของ Azure AD เชื่อมต่อเป็นเวอร์ชันปัจจุบันเสมอ
