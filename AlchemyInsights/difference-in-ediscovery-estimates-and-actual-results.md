---
title: ความแตกต่างในการประมาณ eDiscovery และผลลัพธ์ตามจริง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13997"
- "3200003"
ms.openlocfilehash: e2a1f5ac688adc449286f920d4392adeb3fbd947
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506984"
---
# <a name="difference-in-ediscovery-estimates-and-actual-results"></a>ความแตกต่างในการประมาณ eDiscovery และผลลัพธ์ตามจริง

ถ้าคุณเห็นความแตกต่างระหว่างผลลัพธ์การค้นหาโดยประมาณและผลลัพธ์จริงที่ส่งออกในการค้นหา eDiscovery ของคุณ อาจเป็นสาเหตุของความคลาดเคลื่อน:

- การเปลี่ยนแปลงที่เกิดขึ้นตั้งแต่เวลาที่ประเมินและส่งออกผลลัพธ์
- รายการที่ไม่เป็นดัชนีรวมอยู่ในการส่งออกของคุณ
- ระหว่างการส่งออก การค้นหาจะถูกเรียกใช้อีกครั้งและข้อความจริงจะถูกดึงมาจากExchangeฐานข้อมูล
- รายการที่ไม่เป็นดัชนีSharePointและOneDriveจะไม่รวมอยู่ในการประเมินการค้นหา

For explanations and a list of additional reasons for discrepancies, see [Differences between estimated and actual eDiscovery search results](https://docs.microsoft.com/microsoft-365/compliance/differences-between-estimated-and-actual-ediscovery-search-results).