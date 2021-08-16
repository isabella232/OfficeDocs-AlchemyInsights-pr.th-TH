---
title: จํากัดการเข้าถึงในSharePointหรือOneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075059"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>จํากัดการเข้าถึงในSharePointหรือOneDrive

ในSharePointและOneDrive จํากัดการเข้าถึงรายการต่างๆ เช่น ไฟล์ โฟลเดอร์ และรายการ โดยการให้สิทธิ์การเข้าถึงเฉพาะกลุ่มหรือบุคคลที่คุณต้องการให้มีสิทธิ์เข้าถึงเท่านั้น ตามค่าเริ่มต้น สิทธิ์ในSharePointจะสืบทอดมาจากค่าที่สูงกว่าในล.ก. ดังนั้นไฟล์จะสืบทอดสิทธิ์จากโฟลเดอร์ ซึ่งสืบทอดสิทธิ์จากไลบรารี ซึ่งสืบทอดสิทธิ์จากไซต์
  
You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. อย่างไรก็ตาม เราไม่แนะนนะให้สิ่งนี้เนื่องจากจะรักษาสิทธิ์ให้ซับซ้อนและสับสนมากขึ้นในอนาคต นี่คือสิ่งที่คุณสามารถแก้ไขแทนได้:
  
- ตัวอย่างเช่น ถ้าคุณต้องการแชร์เนื้อหาทั้งหมดของโฟลเดอร์ ยกเว้นไฟล์หนึ่งย้ายไฟล์นั้นไปยังสถานที่ใหม่ที่ไม่ได้แชร์
    
- ถ้าคุณมีโฟลเดอร์ย่อยสองโฟลเดอร์และคุณต้องการแชร์โฟลเดอร์ย่อยหนึ่งโฟลเดอร์กับกลุ่ม A และ B และอนุญาตเฉพาะกลุ่ม A ในการเข้าถึงโฟลเดอร์ย่อยที่สอง แชร์โฟลเดอร์หลักกับกลุ่ม A และเพิ่มกลุ่ม B ลงในโฟลเดอร์ย่อยแรก
    
[หยุดการแชร์ไฟล์หรือโฟลเดอร์ ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

