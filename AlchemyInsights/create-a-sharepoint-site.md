---
title: การสร้างไซต์ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: a4c6029c632178136396a91ba9754752dc8f7180
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32407633"
---
# <a name="create-a-sharepoint-site"></a>การสร้างไซต์ SharePoint

ดูการ[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation )สำหรับตัวเลือกการสร้างไซต์ เลือกเพื่อสร้าง[ไซต์สำหรับทีม](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US)(ซึ่งจะสร้างกลุ่ม Office 365) หรือ[ไซต์การสื่อสาร](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) การสร้าง[ไซต์แบบคลาสสิก](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)หรือไซต์ทีมใหม่ที่ไม่มีกลุ่มที่มี Office 365 คลิก**ตัวเลือกอื่น ๆ** 
  
เคล็ดลับ:
- *คุณไม่สามารถสร้างไซต์ ด้วย URL ของไซต์ที่มีอยู่เดิม ถ้าคุณลบไซต์ และขอให้ใช้ URL อีกครั้ง คุณสามารถได้ในไซต์ที่ถูกลบยังคงอยู่ภายใต้**ไซต์ถูกลบ** จัดการลบไซต์ดู[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) เมื่อต้องการเอาไซต์ ด้วย Powershell ดูตัวอย่างการ cmdlet [SPSite เอา](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)*
- *ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ ดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)*
- *คุณสามารถได้ไซต์ปรากฏขึ้นติดที่**สร้าง**นานกว่าที่คาดไว้ ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์*
