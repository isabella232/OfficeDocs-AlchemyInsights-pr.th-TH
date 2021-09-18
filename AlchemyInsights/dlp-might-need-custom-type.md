---
title: DLP อาจต้องใช้ชนิดแบบเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446710"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจต้องใช้ชนิดแบบเอง

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวทางออนไลน์ เพื่อดูข้อมูลเพิ่มเติม

**DLP อาจต้องใช้ชนิดข้อมูลแบบเอง**

ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่เป็นความลับแบบปรับแต่งเองเพื่อปกป้องข้อมูลองค์กรของคุณ For more information, see [Learn about sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) and Sensitive information type entity [definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

For more information on how to create custom sensitive information types and policies, see: 

**การปรับแต่งชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**

ถ้าชนิดข้อมูลที่เป็นความลับในตัวตรงกับความต้องการของคุณ ที่มีการปรับแต่งเพียงไม่กี่อย่าง ให้ดู [ปรับแต่งชนิดข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)ที่เป็นความลับที่มีอยู่แล้วภายใน ตัวอย่างเช่น คุณสามารถเพิ่มหรือเอาคําหลักออก หรือเพิ่มหรือเอาหลักฐานการสนับสนุนออก เช่น วันที่หรือที่อยู่

**สร้างชนิดข้อมูลที่เป็นความลับแบบเอง**

แต่ถ้าคุณต้องระบุและป้องกันชนิดข้อมูลที่เป็นความลับชนิดอื่นทั้งหมด คุณสามารถสร้างชนิดข้อมูลที่เป็นความลับแบบศูนย์การปฏิบัติตามข้อบังคับสำหรับ Microsoft 365ได้ For more information, see [Get started with custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**สร้างชนิดข้อมูลที่เป็นความลับแบบเองในศูนย์การรักษา&การปฏิบัติตามนโยบายของ PowerShell**

สุดท้าย ถ้าส่วนติดต่อผู้ใช้ไม่ได้ให้ตัวเลือกทั้งหมดที่คุณต้องการ คุณสามารถสร้างชนิดข้อมูลที่เป็นความลับแบบปรับแต่งเองใน Security & Compliance Center PowerShell By starting with an XML file, you can use every option available. For more information, see [Create a custom sensitive information type using PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

เมื่อต้องการทดสอบนโยบายของคุณในโหมดทดสอบก่อน ให้ดู[ใช้นโยบายในโหมดทดสอบ](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode)[และ สร้าง ทดสอบ และปรับนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 