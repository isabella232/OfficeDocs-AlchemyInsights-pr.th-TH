---
title: การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968396"
---
# <a name="changing-ews-throttling-settings"></a>การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS

โปรดเรียกใช้การทดสอบอัตโนมัติของเราซึ่งจะอนุญาตให้คุณปรับเปลี่ยนนโยบายการควบคุมปริมาณ EWS ในช่วงระยะเวลาการโยกย้ายของคุณ โปรดทราบว่าแม้หลังจากเรียกใช้การนําเข้า EWS จะยังคงถูกจํากัดที่ 150mb ต่อ 5 นาทีต่อกล่องจดหมาย เพื่อให้ได้รับความเร็วในการโยกย้ายที่สูงขึ้น โปรดโยกย้ายผู้ใช้มากขึ้นพร้อมกัน

โปรดทราบว่าการเปลี่ยนแปลงนโยบายการควบคุมปริมาณ EWS จะไม่มีผลต่อชนิดการโยกย้ายต่อไปนี้ (โดยใช้เครื่องมือของ Microsoft): แบบไฮบริด, แบบเคลื่อนย้าย/Staged (RPC/HTTP), IMAP, G Suite, โฟลเดอร์สาธารณะ หรือบริการการนําเข้า PST