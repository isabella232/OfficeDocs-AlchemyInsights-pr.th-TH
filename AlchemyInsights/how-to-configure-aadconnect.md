---
title: 646 วิธีการการตั้งค่าคอนฟิก AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856675"
---
# <a name="configure-sync-features"></a>การตั้งค่าคอนฟิกลักษณะการทำข้อมูลให้ตรงกัน

การเชื่อมต่อ AD azure มีคุณลักษณะหลายประการที่จะเปิดใช้งาน โดยค่าเริ่มต้น หรือ ที่คุณสามารถเปิดใช้งานในภายหลัง คุณลักษณะบางอย่างจำเป็นต้องมีการตั้งค่าคอนฟิกเพิ่มเติมในสภาพแวดล้อมที่เฉพาะเจาะจง

- ขีดจำกัด[การกรอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)วัตถุจะซิงโครไนส์เพื่อโฆษณา Azure โดยค่าเริ่มต้น ผู้ใช้ ผู้ติดต่อ กลุ่ม และทั้งหมด Windows 10 บัญชีคอมพิวเตอร์มีการซิงโครไนส์ คุณสามารถรวม หรือไม่รวมวัตถุที่ยึดตามโดเมน Ou หรือแอททริบิวต์อื่น ๆ

- [Syncronization แฮชของรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)ซิงโครไนส์แฮชของรหัสผ่านจากไดเรกทอรีที่ใช้งานอยู่ในสถานที่เพื่อโฆษณา Azure ซึ่งช่วยให้การจัดการรหัสผ่านในสถานหนึ่ง แต่ใช้รหัสผ่านเดียวกันในทั้งสองในสถาน และสภาพแวดล้อมที่ cloud เนื่องจากไดเรกทอรีที่ใช้งานอยู่ไม่เชื่อถือแหล่งที่มา คุณสามารถใช้นโยบายรหัสผ่านของคุณเอง

- [(SSPR) การรีเซ็ตรหัสผ่านด้วยตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)อนุญาตให้ผู้ใช้สามารถรีเซ็ตรหัสผ่านของตนเองใน cloud ขณะที่ยังคง ใช้นโยบายรหัสผ่านของคุณในสถาน

- [เขียนกลับอุปกรณ์](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)ช่วยให้อุปกรณ์ที่ลงทะเบียนใน Azure โฆษณาที่มีการบันทึกกลับไปยัง Active Directory ในสถานเพื่อให้สามารถใช้สำหรับการเข้าถึงแบบมีเงื่อนไข

- [กรณีการป้องกันลบ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)ถูกเปิดใช้งาน โดยค่าเริ่มต้นเพื่อช่วยป้องกันการลบวัตถุพร้อม ๆ กันมากเกินไป (เกินกว่า 500 วัตถุต่อการซิงโครไนส์) คุณสามารถเปลี่ยนการตั้งค่านี้ให้ตรงกับความต้องการขององค์กรของคุณ

- [การอัพเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)ถูกเปิดใช้งาน โดยค่าเริ่มต้นสำหรับการติดตั้งด่วน และช่วยให้แน่ใจว่า เชื่อมต่อ AD Azure รุ่นของคุณเป็นปัจจุบันเสมอ
