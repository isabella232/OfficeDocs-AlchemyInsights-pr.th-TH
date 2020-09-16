---
title: การลบแชนเนลส่วนตัวของทีม
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730934"
---
# <a name="delete-a-teams-private-channel"></a>การลบแชนเนลส่วนตัวของทีม

Microsoft ทราบถึงปัญหาในการลบทีมส่วนตัวถ้าคุณมีนโยบายการเก็บข้อมูล SharePoint ที่เปิดใช้งานสำหรับไซต์ SharePoint ต้นแบบ Microsoft กำลังทำงานกับการแก้ไข ในระหว่างนี้คุณสามารถใช้วิธีการแก้ไขปัญหาต่อไปนี้เพื่อลบช่องทางส่วนตัว

**ยกเว้นไซต์คอลเลกชันของทีม/ไซต์คอลเลกชันจากนโยบายการเก็บข้อมูลของ Sharepoint**

1. ไปที่พอร์ทัลผู้ดูแลระบบ Office ๓๖๕แล้วเลือก **แสดงทั้งหมด** ในบานหน้าต่างนำทางด้านซ้าย
2. ภายใต้**ศูนย์การจัดการ**ให้ไปที่นโยบายการป้องกันการสูญหายของข้อมูลการ**รักษาความปลอดภัย & การปฏิบัติ**ตามนโยบาย  >  **Data Loss Prevention**  >  **Policy**
3. ระบุนโยบายใดๆที่นำไปใช้กับไซต์ Sharepoint และปรับเปลี่ยนนโยบายดังนั้นไซต์ Sharepoint สำหรับทีมที่มีแชนเนลส่วนตัวจะไม่รวมอยู่ภายใต้นโยบายการเก็บข้อมูล
4. บันทึกนโยบาย
    อาจใช้เวลาถึง24ชั่วโมงสำหรับการตั้งค่านโยบายจะมีผล
    หลังจากที่ไซต์ถูกแยกออกแล้วคุณสามารถลบแชนเนลส่วนตัวได้  
    
คุณ  ***อาจ*** สามารถลบช่องทางส่วนตัวโดยใช้ทีม Microsoft บนอุปกรณ์ Android ของคุณ 

สำหรับข้อมูล SharePoint ที่เกี่ยวข้องให้ดูที่ [ไม่สามารถลบรายการใน SharePoint Online หรือ OneDrive For Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)ได้