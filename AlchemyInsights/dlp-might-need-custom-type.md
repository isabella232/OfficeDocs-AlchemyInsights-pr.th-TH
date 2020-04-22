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
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704508"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจต้องการชนิดที่กําหนดเอง

**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม

**DLP อาจต้องการชนิดข้อมูลแบบกําหนดเอง**

ด้วยนโยบายการป้องกันข้อมูลสูญหาย (DLP) คุณจะสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้ ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน**แบบกําหนดเอง**ของคุณเองเพื่อป้องกันข้อมูลองค์กรของคุณ

ตัวอย่างเช่น องค์กรของคุณอาจจําเป็นต้องระบุและป้องกันหมายเลขพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบเฉพาะกับองค์กรของคุณ ถ้าเป็นเช่นนั้น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม
  
 **กําหนดชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**
  
หากชนิดข้อมูลที่สําคัญในตัวจะตอบสนองความต้องการของคุณมีเพียงการปรับแต่งไม่กี่คุณสามารถ[ปรับแต่งในตัวชนิดข้อมูลที่สําคัญ](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type) ตัวอย่างเช่น คุณสามารถเพิ่มหรือนําคําหลักออก หรือเพิ่มหรือลบหลักฐานสนับสนุน เช่น วันที่หรือที่อยู่ออกได้
  
 **สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**
  
แต่ถ้าคุณต้องการระบุและป้องกันข้อมูลที่สําคัญชนิดอื่น &ทั้งหมด[create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
  
**สร้างชนิดข้อมูลที่สําคัญแบบกําหนดเองในการรักษาความปลอดภัย&ศูนย์ควบคุมการปฏิบัติตามกฎระเบียบ PowerShell**

สุดท้ายถ้า UI ไม่ได้ให้ตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถสร้าง[ชนิดข้อมูลที่สําคัญที่กําหนดเองในการรักษาความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell) โดยเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทั้งหมดที่พร้อมใช้งาน
