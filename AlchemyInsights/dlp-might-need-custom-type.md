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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030813"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจต้องใช้ชนิดแบบเอง

**สิ่ง** สําคัญ: ในระหว่างช่วงเวลาที่ไม่มีประวัติใช้งานเหล่านี้ เราปฏิบัติตามขั้นตอนต่างๆ เพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานอยู่ โปรดเยี่ยมชม SharePoint [การปรับ](https://aka.ms/ODSPAdjustments)ฟีเจอร์ชั่วคราวแบบออนไลน์ SharePoint เพื่อดูข้อมูลเพิ่มเติม

**DLP อาจต้องใช้ชนิดข้อมูลแบบเอง**

ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่เป็นความลับ **แบบปรับแต่ง** เองเพื่อปกป้องข้อมูลองค์กรของคุณ

ตัวอย่างเช่น องค์กรของคุณอาจต้องการระบุและปกป้องรหัสพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบที่เฉพาะเจาะจงกับองค์กรของคุณ ถ้าเป็นดังนั้น ให้ดูบทความต่อไปนี้เพื่อดูข้อมูลเพิ่มเติม
  
 **การปรับแต่งชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**
  
ถ้าชนิดข้อมูลที่เป็นความลับในตัวตรงกับความต้องการของคุณ มีเพียงปรับแต่งเล็กน้อย คุณสามารถปรับแต่งชนิดข้อมูลที่เป็นความลับ[ที่มีอยู่แล้วภายในได้](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) ตัวอย่างเช่น คุณสามารถเพิ่มหรือเอาคําหลักออก หรือเพิ่มหรือเอาหลักฐานการสนับสนุนออก เช่น วันที่หรือที่อยู่
  
 **สร้างชนิดข้อมูลที่เป็นความลับแบบเอง**
  
แต่ถ้าคุณต้องระบุและป้องกันชนิดข้อมูลที่ละเอียดอ่อนชนิดอื่นทั้งหมด คุณสามารถสร้างชนิดข้อมูลที่เป็นความลับแบบปรับแต่งเองใน[](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)UI ของศูนย์การรักษา&การปฏิบัติตามนโยบาย
  
**สร้างชนิดข้อมูลที่เป็นความลับแบบปรับแต่งเองใน ศูนย์&การปฏิบัติตามนโยบายของ PowerShell**

สุดท้าย ถ้า UI ไม่มีตัวเลือกทั้งหมดที่คุณต้องการ คุณสามารถสร้างชนิดข้อมูลที่เป็นความลับแบบปรับแต่งเองใน ศูนย์การรักษา&[ปฏิบัติตามนโยบายของ PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) By starting with an XML file, you can use every option available.
