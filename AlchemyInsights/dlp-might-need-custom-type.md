---
title: DLP อาจต้องการชนิดที่กําหนดเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507533"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจต้องการชนิดที่กําหนดเอง

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**DLP อาจต้องการชนิดข้อมูลที่กําหนดเอง**

ด้วยนโยบายการป้องกันข้อมูลสูญหาย (DLP) คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน**แบบกําหนดเอง**เพื่อปกป้องข้อมูลขององค์กร

ตัวอย่างเช่น องค์กรของคุณอาจจําเป็นต้องระบุและป้องกันรหัสพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบเฉพาะขององค์กรของคุณ ถ้าเป็นเช่นนั้น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม
  
 **กําหนดชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**
  
หากข้อมูลที่สําคัญในตัวจะตอบสนองความต้องการของคุณมีเพียงการปรับแต่งไม่กี่, คุณสามารถกําหนด[ในตัวประเภทข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). ตัวอย่างเช่น คุณสามารถเพิ่มหรือลบคําหลัก หรือเพิ่มหรือลบหลักฐานการสนับสนุน เช่น วันที่หรือที่อยู่
  
 **สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**
  
แต่ถ้าคุณต้องการระบุและป้องกันข้อมูลที่สําคัญชนิดอื่น &ทั้งหมด[create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)
  
**สร้างชนิดข้อมูลที่สําคัญแบบกําหนดเองในความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ PowerShell**

สุดท้ายถ้า UI ไม่ได้มีตัวเลือกทั้งหมดที่คุณต้องการ[คุณสามารถสร้างชนิดข้อมูลที่สําคัญที่กําหนดเองในการรักษาความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) โดยเริ่มต้นด้วยไฟล์ XML คุณสามารถใช้ทุกตัวเลือกที่มีอยู่
