---
title: การสร้างนโยบายป้ายชื่อ AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: d24696b63663c69b22c783072141af62ecf124dba7b49bca827381f39f88640e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032001"
---
# <a name="creating-aip-label-policies"></a>การสร้างนโยบายป้ายชื่อ AIP

ป้ายชื่อ Azure Information Protection(AIP) สามารถใช้กับข้อมูลช่วงข้อมูลทั้งหมดที่โดยปกติแล้วองค์กรจะสร้างและจัดเก็บ จากการจัดประเภทข้อมูลส่วนบุคคลต่สุด ไปยังการจัดประเภทสูงสุดของข้อมูลที่เป็นความลับสูง นโยบายการปกป้องข้อมูล Azure จะมีผลบังคับใช้กับไคลเอ็นต์แบบคลาสสิกของ Azure Information Protection(AIP) และไม่ใช่ไคลเอ็นต์[ป้ายผนึกแบบรวมของ AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) คุณสามารถกําหนดค่าหลายองค์ประกอบในนโยบาย AIP ได้ รวมถึงตัวเลือกต่างๆ เช่น:

- ตัวเลือกป้ายชื่อที่จะให้ผู้ดูแลระบบหรือผู้ใช้จัดประเภทและป้องกัน(ไม่บังคับ) เอกสารและอีเมล
- ตัวเลือกในการบังคับใช้การจัดประเภทเมื่อผู้ใช้บันทึกเอกสารและส่งอีเมล
- ตัวเลือกในการใส่ป้ายชื่อข้อความอีเมลโดยอัตโนมัติโดยยึดตามสิ่งที่แนบมาของข้อความอีเมลนั้น
- ตัวเลือกในการควบคุมว่าแถบการป้องกันข้อมูลจะแสดงในOfficeหรือไม่

For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).  

ดูแหล่งข้อมูลที่เป็นประโยชน์อื่นๆ เกี่ยวกับนโยบาย AIP ที่:

- [บทช่วยสอน: กําหนดการตั้งค่านโยบาย Azure Information Protection และสร้างป้ายชื่อใหม่](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [การกําหนดค่านโยบาย Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [สร้างและกําหนดค่าป้ายระดับความลับและนโยบายของป้ายก่านั้น](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [คู่มือวิธีการเกี่ยวกับสถานการณ์ทั่วไปที่ใช้ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [ตรวจทานเอกสาร Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [ความต้องการของ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [บทช่วยสอนเริ่มต้นใช้งานด่วนของ Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [ดาวน์โหลดไคลเอ็นต์ Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)