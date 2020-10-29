---
title: ไฟล์ตามความต้องการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791313"
---
# <a name="configure-files-on-demand"></a>กำหนดค่าไฟล์ตามความต้องการ

ไฟล์ OneDrive ตามความต้องการต้องการการ [อัปเดต windows 10](https://go.microsoft.com/fwlink/p/?linkid=859040) (เวอร์ชัน๑๗๐๙หรือใหม่กว่า) หรือ windows Server ๒๐๑๙และ OneDrive รุ่น17.3.7064.1005 หรือเวอร์ชันที่ใหม่กว่า

ไฟล์ OneDrive ตามความต้องการของคุณจะช่วยให้คุณสามารถเข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive ได้โดยไม่ต้องดาวน์โหลดทั้งหมดและใช้พื้นที่เก็บข้อมูลบนอุปกรณ์ของคุณ

เมื่อต้องการกำหนดค่าไฟล์ตามความต้องการบนพีซีของคุณ:

1. เลือกไอคอนรูปเมฆสีขาวหรือสีน้ำเงินของ **OneDrive** ในพื้นที่แจ้งให้ทราบของแถบงาน Windows เลือก **วิธีใช้ &** ไอคอนเกียร์การตั้งค่า > **การตั้งค่า**
2. บนแท็บ **การตั้งค่า** ให้เลือก **บันทึกช่องว่างและดาวน์โหลดไฟล์ขณะที่คุณใช้กล่องเหล่านั้น**  

นอกจากนี้คุณยังสามารถกำหนดค่าไฟล์ตามความต้องการโดยใช้รีจิสทรีได้อีกด้วย

ถ้าคุณปิดใช้งานการตั้งค่านี้ผู้ใช้ Windows 10 จะมีลักษณะการทำงานการซิงค์เดียวกันกับผู้ใช้ Windows เวอร์ชันก่อนหน้าและไม่สามารถเปิดไฟล์ตามความต้องการได้ ถ้าคุณไม่ได้กำหนดค่าการตั้งค่านี้ผู้ใช้สามารถเปิดหรือปิดไฟล์ตามความต้องการได้

การเปิดใช้งานนโยบายนี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น1 การปิดใช้งานนโยบายนี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น0

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

ถ้าคุณไม่เห็นตัวเลือกไฟล์ตามความต้องการใน "การตั้งค่า" ให้ตรวจสอบให้แน่ใจว่าชนิดเริ่มต้นของบริการ "Windows Cloud Files Filter Driver" ถูกตั้งค่าเป็น 2 (AUTO_START) การเปิดใช้งานฟีเจอร์นี้จะตั้งค่าคีย์รีจิสทรีต่อไปนี้เป็น2

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`