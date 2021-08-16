---
title: ทดสอบความเข้ากันได้ของแอป
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 40c16324270e26a882b16e5c2e0a6cf248d34ed84e95e845aac5dfa44ac58c72
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004853"
---
# <a name="do-app-compatibility-testing"></a>ทดสอบความเข้ากันได้ของแอป

ความเข้ากันได้ของแอปพลิเคชันMicrosoft Edgeอยู่ในระดับสูงมาก อันที่จริง Microsoft ให้สัญญาว่าจะเข้ากันได้กับสิ่งต่อไปนี้:
- หากใช้งานได้กับ Microsoft Edge 45 และเวอร์ชันก่อนหน้า จะใช้งานได้ใน Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า
- หากสามารถใช้งานบน Internet Explorer ได้ จะMicrosoft Edgeในโหมด Internet Explorer
- หากใช้งานได้บน Google Chrome แอปจะMicrosoft Edgeได้

ถ้าคุณมีแอปพลิเคชันที่เราไม่ตรงกับสัญญานี้ เราจะสัญญาว่าจะแก้ไขด้วย[Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)

แม้ว่าจะสัญญานี้ เราทราบว่าหลายองค์กรต้องตรวจสอบแอปพลิเคชันบางรายการเพื่อเหตุผลในการปฏิบัติตามกฎข้อบังคับหรือการจัดการความเสี่ยง แม้ว่าเราจะคิดว่านี่จะไม่ง่ายเลย แต่การจัดระเบียบและเข้มงวดในการทดสอบแอปก็เป็นเรื่องสําคัญ

มีสองวิธีในการทดสอบความเข้ากันได้ของแอป:

- **การทดสอบแล็บ**: แอปพลิเคชันได้รับการทดสอบในสภาพแวดล้อมที่ควบคุมอย่างแน่นหนาด้วยการกําหนดค่าเฉพาะ
- **การทดสอบการทดสอบทดสอบ** ร่อง : แอปพลิเคชันได้รับการทดสอบโดยผู้ใช้จํานวนจํากัดในสภาพแวดล้อมการงานในแต่ละวันโดยใช้อุปกรณ์ของตนเอง

เลือกวิธีการที่เหมาะสมที่สุดของแต่ละแอปและทดสอบก่อนที่จะเปิดใช้ทั้งองค์กร

เมื่อคุณมั่นใจว่าแอปของคุณเข้ากันได้ คุณก็พร้อมที่จะปรับใช้Microsoft Edgeกลุ่มทดลอง
