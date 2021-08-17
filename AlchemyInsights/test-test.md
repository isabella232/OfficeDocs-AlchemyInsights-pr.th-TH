---
title: ข้อใดที่หายไปSharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106451"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intun1

นโยบายการป้องกันปลายทางของ Intunes สามารถใช้เพื่อกําหนดค่าการตั้งค่าการเข้ารหัสลับ Boitlocker Windows ตามที่อธิบายไว้ในการตั้งค่า : Windows10 (และใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intunes

คุณควรทราบว่าอุปกรณ์ที่ใหม่กว่าหลายเครื่องWindows 10การเข้ารหัสลับ bitlocker อัตโนมัติซึ่งจะถูกทริกเกอร์โดยไม่มีแอปพลิเคชันนโยบาย MDM ซึ่งอาจส่งผลกระทบต่อแอปพลิเคชันของนโยบายถ้ามีการกําหนดค่าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้น ดู FAQ เพื่อดูรายละเอียดเพิ่มเติม


Q:ถามที่ถามบ่อย: Windowsรุ่นใดสนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันจุดสิ้นสุด
A: การตั้งค่าในนโยบายการป้องกันจุดสิ้นสุดของ Intuned จะถูกปรับใช้โดยใช้ Bitlocker CSP  มีไม่ทุกรุ่นหรือรุ่นWindows Bitlocker CSP ขณะนี้Windows: องค์กร Education, Mobile, Mobile Enterprise และ Professional (ตั้งแต่รุ่น 1809 เป็นต้นไป) ได้รับการสนับสนุน




Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของ OS ในวิธีการเข้ารหัสลับและจุดแข็งการเข้ารหัส (XTS-AES-128) จะปรับใช้นโยบายกับการตั้งค่าอื่นทริกเกอร์การเข้ารหัสลับไดรฟ์ใหม่ด้วยการตั้งค่าใหม่โดยอัตโนมัติหรือไม่

A: ไม่ได้ เมื่อต้องการใช้การตั้งค่ารหัสใหม่ ไดรฟ์จะต้องถอดรหัสลับก่อน

หมายเหตุ For devices being enrolled with Autopilot the automatic encryption that would would occur during OOBE is not triggered until Intuned policy is evaluated which allows the policy based settings to be used in place of the OS defaults




Q ถ้าอุปกรณ์ถูกเข้ารหัสลับเนื่องจากแอปพลิเคชันนโยบาย Intuned จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่

A: การเอานโยบายที่เกี่ยวข้องกันของการเข้ารหัสลับออกจะไม่ส่งผลให้มีการเข้ารหัสลับไดรฟ์ที่ถูกกําหนดค่าไว้




Q: เหตุใดนโยบายการปฏิบัติตามข้อบังคับ Intun1 จึงแสดงให้เห็นว่าอุปกรณ์ของฉันไม่มี "เปิดใช้งาน Bitlocker" แต่เป็น

A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบาย intuned Windows Device Health Attestation (DHA) ไคลเอ็นต์นี้วัดสถานะอุปกรณ์เมื่อเริ่มระบบเท่านั้น ดังนั้นถ้ายังไม่ได้เริ่มต้นระบบใหม่เนื่องจากการเข้ารหัสลับ Bitlocker เสร็จสมบูรณ์ บริการไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ว่าใช้งานอยู่