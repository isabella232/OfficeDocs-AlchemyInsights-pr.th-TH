---
title: 646วิธีการกําหนดค่า AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722582"
---
# <a name="configure-sync-features"></a>กําหนดค่าคุณลักษณะการซิงค์

การเชื่อมต่อ AD Azure มีคุณลักษณะหลายอย่างที่เปิดใช้งาน โดยค่าเริ่มต้น หรือที่คุณสามารถเปิดใช้งานในภายหลัง คุณลักษณะบางอย่างจําเป็นต้องมีการกําหนดค่าเพิ่มเติมในสภาพแวดล้อมเฉพาะ

- [การกรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)จํากัดวัตถุจะซิงโครไนส์กับโฆษณา Azure โดยค่าเริ่มต้น ผู้ใช้ทั้งหมด ผู้ติดต่อ กลุ่ม และ Windows 10 บัญชีคอมพิวเตอร์จะซิงโครไนส์ คุณสามารถรวมหรือแยกวัตถุตามโดเมน, OUs หรือแอตทริบิวต์อื่นๆ ได้

- [ซิงโครไนส์แฮรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)แฮซิงโครไนส์แฮรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อโฆษณา Azure วิธีนี้ช่วยให้การจัดการรหัสผ่านอยู่ในตําแหน่งเดียว แต่ใช้รหัสผ่านเดียวกันทั้งในสภาพแวดล้อมภายในและระบบคลาวด์ เนื่องจาก Active Directory เป็นแหล่งที่เชื่อถือได้ คุณจึงสามารถใช้นโยบายรหัสผ่านของคุณเองได้

- [การรีเซ็ตรหัสผ่านด้วยตนเอง (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)ช่วยให้ผู้ใช้สามารถรีเซ็ตรหัสผ่านของตนเองในระบบคลาวด์ในขณะที่ยังคงใช้นโยบายรหัสผ่านในสถานที่ของคุณ

- [อุปกรณ์ writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)ช่วยให้อุปกรณ์ที่ลงทะเบียนในโฆษณา Azure จะถูกเขียนกลับไปยังไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อให้สามารถใช้สําหรับการเข้าถึงแบบมีเงื่อนไข

- [ป้องกันการลบโดยไม่ตั้งใจ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)ถูกเปิดใช้งานโดยค่าเริ่มต้นเพื่อช่วยป้องกันการลบวัตถุพร้อมกันมากเกินไป (มากกว่า 500 วัตถุต่อการทําข้อมูลให้ตรงกัน) คุณสามารถเปลี่ยนการตั้งค่านี้ให้ตรงกับความต้องการขององค์กรของคุณ

- [การปรับรุ่นอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)ถูกเปิดใช้งานโดยค่าเริ่มต้นสําหรับการติดตั้งแบบด่วน และช่วยให้มั่นใจว่ารุ่นของการเชื่อมต่อ AD Azure เป็นรุ่นล่าสุดอยู่เสมอ
