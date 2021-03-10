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
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694860"
---
# <a name="do-app-compatibility-testing"></a>ทดสอบความเข้ากันได้ของแอป

ความเข้ากันได้ของแอปพลิเคชันของ Microsoft Edge สูงมาก ที่จริงแล้ว Microsoft ให้สัญญาว่าจะมีความเข้ากันได้ดังต่อไปนี้:
- หากใช้งานได้กับ Microsoft Edge 45 และเวอร์ชันก่อนหน้า จะใช้งานได้กับ Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า
- หากสามารถใช้งานบน Internet Explorer ได้ ก็จะสามารถใช้งานบน Microsoft Edge ในโหมด Internet Explorer ได้
- หากสามารถใช้งานบน Google Chrome ได้ ก็จะสามารถใช้งานบน Microsoft Edge ได้

ถ้าคุณมีแอปพลิเคชันที่เราไม่เป็นไปตามสัญญานี้ เราจะสัญญาว่าจะแก้ไขด้วย[Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)

แม้ว่าจะสัญญานี้ เราทราบว่าหลายองค์กรต้องตรวจสอบแอปพลิเคชันบางรายการด้วยเหตุผลด้านการปฏิบัติตามกฎข้อบังคับหรือการจัดการความเสี่ยง แม้ว่าเราคาดหวังว่าสิ่งนี้จะเป็นเรื่องที่ง่ายมาก แต่การจัดระเบียบและอย่างเข้มงวดในการทดสอบแอปก็เป็นเรื่องสําคัญ

มีสองวิธีในการทดสอบความเข้ากันได้ของแอป:

- **การทดสอบแล็บ**: แอปพลิเคชันได้รับการทดสอบในสภาพแวดล้อมที่ควบคุมอย่างแน่นหนาด้วยการกําหนดค่าเฉพาะ
- **การทดสอบการทดสอบร่อง**: แอปพลิเคชันได้รับการทดสอบโดยผู้ใช้จํานวนจํากัดในสภาพแวดล้อมการงานในแต่ละวันโดยใช้อุปกรณ์ของตนเอง

เลือกวิธีการที่เหมาะสมที่สุดในแต่ละแอป และทดสอบก่อนที่จะเปิดใช้ทั้งองค์กร

เมื่อคุณมั่นใจได้ว่าแอปของคุณเข้ากันได้ คุณก็พร้อมที่จะปรับใช้ Microsoft Edge กับกลุ่มทดลอง
