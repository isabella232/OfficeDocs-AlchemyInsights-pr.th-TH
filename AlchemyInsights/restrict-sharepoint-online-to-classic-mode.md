---
title: จํากัด SharePoint แบบออนไลน์เป็นโหมดคลาสสิก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742488"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>จํากัด SharePoint แบบออนไลน์เป็นโหมดคลาสสิก

บางองค์กรยังคงต้องการประสบการณ์การใช้งานโหมดคลาสสิก ในขณะที่ไม่มีแผนที่จะเอาโหมดคลาสสิกในระดับระดับย่อย, มันเป็นไปไม่ได้ที่จะ จํากัด ทั้งองค์กร (ผู้เช่า) ไปยังโหมดคลาสสิกสําหรับรายการและห้องสมุด.

ผู้ดูแลระบบจะมีตัวเลือกต่อไปนี้ในการจัดการรายการและไลบรารีแต่ละรายการในโหมดคลาสสิกโดยใช้สวิตช์เลือกออกแบบละเอียดที่เราให้อยู่ในระดับต่อไปนี้:

- ไซต์คอลเลกชัน
- ไซต์
- รายการ
- ไลบ รา รี

นอกจากนี้ รายการที่ใช้คุณลักษณะบางอย่างและการกําหนดค่าเองที่ไม่ได้รับการสนับสนุนโดยสมัยใหม่จะยังคงถูกสลับไปยังโหมดคลาสสิกโดยอัตโนมัติ

เริ่มต้น 1 เมษายน 2019 กระบวนการปิดการใช้งานระดับผู้เช่าเลือกออกจากรายการและไลบรารีที่ทันสมัยจะเริ่มต้น และดําเนินต่อถึง 31 พฤษภาคม 2019  รายการและไลบรารีที่อยู่ในโหมดคลาสสิกเนื่องจากผู้ใช้ผู้เช่าไม่รับจะถูกเลื่อนไปยังที่ทันสมัยโดยอัตโนมัติ

หากคุณต้องการโหมดคลาสสิกโปรดดูข้อมูลเพิ่มเติม[ที่นี่](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)และการเรียนการสอน Powershell PnP[ที่นี่](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)ที่อธิบายตัวเลือกและเครื่องมือที่คุณสามารถใช้ในวันนี้เพื่อใช้ประสบการณ์โหมดคลาสสิก
