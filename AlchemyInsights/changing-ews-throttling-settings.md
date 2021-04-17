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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818055"
---
# <a name="changing-ews-throttling-settings"></a>การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS

โปรดเรียกใช้การทดสอบอัตโนมัติของเราซึ่งจะอนุญาตให้คุณปรับเปลี่ยนนโยบายการควบคุมปริมาณ EWS ในช่วงระยะเวลาการโยกย้ายของคุณ โปรดทราบว่าแม้หลังจากเรียกใช้การนําเข้า EWS จะยังคงถูกจํากัดที่ 150mb ต่อ 5 นาทีต่อกล่องจดหมาย เพื่อให้ได้รับความเร็วในการโยกย้ายที่สูงขึ้น โปรดโยกย้ายผู้ใช้มากขึ้นพร้อมกัน

โปรดทราบว่าการเปลี่ยนแปลงนโยบายการควบคุมปริมาณ EWS จะไม่มีผลต่อชนิดการโยกย้ายต่อไปนี้ (โดยใช้เครื่องมือของ Microsoft): แบบไฮบริด, แบบเคลื่อนย้าย/Staged (RPC/HTTP), IMAP, G Suite, โฟลเดอร์สาธารณะ หรือบริการการนําเข้า PST