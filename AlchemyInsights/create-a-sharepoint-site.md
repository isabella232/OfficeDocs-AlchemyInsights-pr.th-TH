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
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802985"
---
# <a name="create-a-sharepoint-site"></a>การสร้างไซต์ SharePoint

คุณสามารถดูที่ด้านล่างสำหรับข้อมูลเกี่ยวกับการสร้างไซต์ SharePoint:
- [จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-site-creation): การเรียนรู้เกี่ยวกับตัวเลือกการสร้างไซต์ รวมทั้งวิธีการสร้างไซต์แบบคลาสสิคหรือไซต์ทีมงานที่ไม่มีกลุ่มที่มี Office 365
- [การสร้างไซต์ทีม SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): การเรียนรู้วิธีการสร้างไซต์สำหรับทีม
- [สร้างไซต์สื่อสารใน SharePoint แบบออนไลน์](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): เรียนรู้วิธีการสร้างไซต์สื่อสาร
- [จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): การเรียนรู้วิธีการสร้างไซต์แบบคลาสสิคหรือไซต์สำหรับทีมที่ไม่มีกลุ่มที่มี Office 365


  
> [! คำแนะนำ]
> - คุณไม่สามารถสร้างไซต์ ด้วย URL ของไซต์ที่มีอยู่เดิม ถ้าคุณลบไซต์ และขอให้ใช้ URL อีกครั้ง คุณสามารถได้ในไซต์ที่ถูกลบยังคงอยู่ภายใต้**ไซต์ถูกลบ** จัดการลบไซต์ดู[ลบไซต์](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) เมื่อต้องการเอาไซต์ ด้วย Powershell ดูตัวอย่างการ cmdlet [SPSite เอา](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
> - ผู้ใช้บางรายอาจไม่สามารถสร้างไซต์ ดู[การสร้างไซต์การจัดการใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/manage-site-creation)
> - คุณสามารถได้ไซต์ปรากฏขึ้นติดที่**สร้าง**นานกว่าที่คาดไว้ ถ้ามากกว่า 24 ชั่วโมงได้ตั้งแต่คุณเห็นปัญหานี้ขั้นแรก โปรดเข้าสู่ระบบ ticket สนับสนุน ในหลายกรณี เรากำลังทำงานอยู่ในโซลูชัน โปรดให้กับเราอย่างน้อย 24 ชั่วโมงในการแก้ไขปัญหาการทำให้เสร็จสมบูรณ์
> - ถ้าคุณต้องการสร้างไซต์ทีมใหม่ที่ไม่มีกลุ่มที่มี Office 365 


