---
title: ลบแชนเนลส่วนตัวของทีม
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439912"
---
# <a name="delete-a-teams-private-channel"></a>ลบแชนเนลส่วนตัวของทีม

Microsoft ตระหนักถึงปัญหาในการลบแชนเนลส่วนตัวของ Teams ถ้าคุณมีนโยบายการเก็บข้อมูล SharePoint ที่เปิดใช้งานสําหรับไซต์ SharePoint ต้นแบบ ไมโครซอฟท์กําลังทํางานเกี่ยวกับการแก้ไข ในระหว่างนี้ คุณสามารถใช้วิธีแก้ปัญหาต่อไปนี้เพื่อลบสถานีส่วนตัว

**แยกชุดทีม/ไซต์ออกจากนโยบายการเก็บข้อมูลของ Sharepoint**

1. ไปที่พอร์ทัลผู้ดูแลระบบ Office 365 แล้วเลือก**แสดงทั้งหมด**ในบานหน้าต่างนําทางด้านซ้าย
2. ภายใต้**ศูนย์การจัดการ**ให้ไปที่**นโยบายการป้องกัน**  >  **การสูญหายของข้อมูล**  >  **Policy**&การปฏิบัติตามกฎระเบียบ
3. ระบุนโยบายใด ๆ ที่ใช้กับไซต์ Sharepoint และปรับเปลี่ยนนโยบายเพื่อให้ไซต์ Sharepoint สําหรับทีมที่มีแชนเนลส่วนตัวไม่ได้รวมอยู่ในนโยบายการเก็บข้อมูล
4. บันทึกนโยบาย
    การตั้งค่านโยบายอาจใช้เวลาถึง 24 ชั่วโมง
    หลังจากที่เว็บไซต์ได้รับการยกเว้นคุณสามารถลบช่องส่วนตัว  
    
***คุณอาจ***ลบช่องส่วนตัวได้โดยใช้ Microsoft Teams บนอุปกรณ์ Android ของคุณ 

สําหรับข้อมูล SharePoint ที่เกี่ยวข้อง ให้ดูที่[ไม่สามารถลบรายการใน SharePoint แบบออนไลน์ หรือ OneDrive สําหรับธุรกิจ](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)