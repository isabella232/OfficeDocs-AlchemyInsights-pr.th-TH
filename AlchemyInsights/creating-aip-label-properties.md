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
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732194"
---
# <a name="creating-aip-label-policies"></a>การสร้างนโยบายป้ายชื่อ AIP

ป้ายชื่อการป้องกันข้อมูลของ Azure (AIP) สามารถใช้กับข้อมูลทั้งหมดที่องค์กรจะสร้างและจัดเก็บจากการจัดประเภทของข้อมูลส่วนบุคคลที่ต่ำที่สุดไปจนถึงการจัดประเภทของข้อมูลที่เป็นความลับสูงสุด นโยบายการป้องกันข้อมูลของ azure จะนำไปใช้กับไคลเอ็นต์การป้องกันข้อมูล Azure (AIP) และไม่ใช่[ไคลเอ็นต์การติดฉลาก Aip Unified](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) คุณสามารถกำหนดค่าองค์ประกอบหลายองค์ประกอบในนโยบาย AIP รวมถึงตัวเลือกต่างๆเช่น:

- ตัวเลือกสำหรับป้ายชื่อใดที่จะช่วยให้ผู้ดูแลระบบหรือการจัดประเภทผู้ใช้และการป้องกัน (ไม่จำเป็น) เอกสารและอีเมล
- ตัวเลือกในการบังคับใช้การจัดประเภทเมื่อผู้ใช้บันทึกเอกสารและส่งอีเมล
- ตัวเลือกในการป้ายชื่อข้อความอีเมลโดยยึดตามสิ่งที่แนบมาโดยอัตโนมัติ
- ตัวเลือกในการควบคุมว่าจะแสดงแถบการป้องกันข้อมูลในแอปพลิเคชัน Office หรือไม่

สำหรับตัวเลือกเพิ่มเติมและข้อมูลเกี่ยวกับนโยบายการป้องกันข้อมูลของ Azure ให้ดูที่:[ภาพรวมของนโยบายการป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/overview-policy)  

สำหรับแหล่งข้อมูลอื่นๆที่มีประโยชน์เกี่ยวกับนโยบายของ AIP ให้ดูที่:

- [บทช่วยสอน: กำหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [การกำหนดค่านโยบายการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [การสร้างและกำหนดค่าป้ายชื่อความลับและนโยบายของพวกเขา](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [เส้นบอกแนววิธีการสำหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [ข้อกำหนดสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure](https://www.microsoft.com/download/details.aspx?id=53018)