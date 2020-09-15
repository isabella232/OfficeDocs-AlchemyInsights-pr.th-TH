---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685617"
---
# <a name="blocking-legacy-authentication"></a>การบล็อกการรับรองความถูกต้องแบบดั้งเดิม

การรับรองความถูกต้องแบบดั้งเดิมคือคำที่อ้างอิงถึงคำขอการรับรองความถูกต้องที่ทำโดย:

- ไคลเอ็นต์ Office รุ่นเก่าที่ไม่ได้ใช้การรับรองความถูกต้องแบบสมัยใหม่ (ตัวอย่างเช่นไคลเอ็นต์ Office ๒๐๑๐)

- ไคลเอ็นต์ใดๆที่ใช้โพรโทคอลของจดหมายแบบดั้งเดิมเช่น IMAP/SMTP/POP3

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการบล็อกการรับรองความถูกต้องแบบดั้งเดิมและการเปิดใช้งานการรับรองความถูกต้องแบบใหม่ให้ดูที่การ[บล็อกการรับรอง](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

ค่าเริ่มต้นของความปลอดภัยใน Azure Active Directory (Azure AD) ทำให้ง่ายต่อการรักษาความปลอดภัยและช่วยปกป้ององค์กรของคุณ ค่าเริ่มต้นของความปลอดภัยมีการตั้งค่าความปลอดภัยที่กำหนดไว้ล่วงหน้าสำหรับการโจมตีทั่วไป
สำหรับข้อมูลเพิ่มเติมเกี่ยวกับค่าเริ่มต้นด้านความปลอดภัยให้ดูที่[ค่าเริ่มต้นด้านความปลอดภัยคืออะไร](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหรือหลังจากวันที่22ตุลาคม๒๐๑๙อาจเป็นไปได้ว่าคุณกำลังประสบกับลักษณะการทำงานที่มีการรักษาความปลอดภัยใหม่และมีค่าเริ่มต้นของความปลอดภัยที่เปิดใช้งานในผู้เช่าของคุณแล้ว  ในความพยายามที่จะปกป้องผู้ใช้ทั้งหมดของเราค่าเริ่มต้นการรักษาความปลอดภัยจะถูกยกเลิกไปยังผู้เช่าใหม่ทั้งหมดที่สร้างขึ้น
