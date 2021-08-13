---
title: จํากัดSharePointออนไลน์เป็นโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958820"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>จํากัดSharePointออนไลน์เป็นโหมดคลาสสิก

บางองค์กรยังคงต้องการประสบการณ์โหมดคลาสสิก ในขณะที่ไม่มีแผนที่จะลบโหมดคลาสสิกในระดับ Granular คุณจะไม่สามารถจํากัดทั้งองค์กร (ผู้เช่า) ให้อยู่ในโหมดคลาสสิกของรายการและไลบรารีได้อีกต่อไป

ผู้ดูแลระบบจะมีตัวเลือกที่ต่อไปนี้เพื่อจัดการรายการและไลบรารีแต่ละรายการในโหมดคลาสสิกโดยใช้สวิตช์การเลือกไม่รับแบบละเอียดที่เรามีในระดับต่อไปนี้:

- ไซต์คอลเลกชัน
- ไซต์
- รายการ
- ไลบรารี

นอกจากนี้ รายการที่ใช้ฟีเจอร์และการการปรับแต่งบางอย่างที่ไม่ได้รับการสนับสนุนโดยสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ

เริ่มตั้งแต่วันที่ 1 เมษายน 2019 กระบวนการปิดใช้งานระดับผู้เช่าที่ปฏิเสธการเข้าร่วมรายการและไลบรารีสมัยใหม่จะเริ่มและต่อเนื่องจนถึงวันที่ 31 พฤษภาคม 2019  รายการและไลบรารีที่อยู่ในโหมดคลาสสิกเนื่องจากการเลือกไม่เข้าร่วมผู้เช่าจะถูกเปลี่ยนเป็นสมัยใหม่โดยอัตโนมัติ

ถ้าคุณต้องใช้โหมดคลาสสิก โปรดดูข้อมูลเพิ่มเติมที่นี่ และ [แ](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) นะนยการใช้งาน Powershell PnP [ที่นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) ที่อธิบายตัวเลือกและเครื่องมือที่คุณสามารถใช้วันนี้เพื่อใช้ประสบการณ์โหมดคลาสสิก
