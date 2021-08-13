---
title: ไฟล์ออนดีมานด์
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
ms.openlocfilehash: 10efdb5e1a90b3e279b8e1716e66a544d0ee34465245f5670930d8a9364a8cc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53977460"
---
# <a name="configure-files-on-demand"></a>กําหนดค่าไฟล์ได้ตามต้องการ

OneDrive การเข้าถึงไฟล์ได้ตามWindows 10 Fall Creators Update [(เวอร์ชัน](https://go.microsoft.com/fwlink/p/?linkid=859040)1709 หรือใหม่กว่า) หรือ Windows Server 2019 และ OneDrive บิลด์ 17.3.7064.1005 หรือใหม่กว่า

OneDrive การเข้าถึงไฟล์ได้ตามต้องการ ช่วยให้คุณเข้าถึงไฟล์OneDriveไฟล์ของคุณได้โดยไม่ต้องดาวน์โหลดไฟล์ทั้งหมดและใช้พื้นที่จัดเก็บบนอุปกรณ์ของคุณ

เมื่อต้องการกําหนดค่า Files On-Demand บนพีซีของคุณ:

1. เลือกไอคอนรูปเมฆ **OneDrive** หรือสีขาวบนระบบคลาวด์Windowsพื้นที่การแจ้งเตือนของแถบงาน เลือก **วิธีใช้ & การตั้งค่า** เกียร์ **>การตั้งค่า**
2. บนแท็บ **การตั้งค่า** เลือก **กล่อง ประหยัดพื้นที่และดาวน์โหลดไฟล์** เมื่อคุณใช้  

คุณยังสามารถกําหนดค่า Files On-Demand โดยใช้รีจิสทรีได้

ถ้าคุณปิดใช้งานการตั้งค่านี้ Windows 10ผู้ใช้จะซิงค์แบบเดียวกับผู้ใช้ Windows เวอร์ชันก่อนหน้า และจะไม่สามารถเปิดการเข้าถึงไฟล์ได้ตามต้องการ ถ้าคุณไม่ได้กําหนดค่าการตั้งค่านี้ ผู้ใช้สามารถเปิดหรือปิด Files On-Demand ได้

การเปิดใช้งานนโยบายนี้จะตั้งค่ารีจิสทรีคีย์ต่อไปนี้เป็น 1 การปิดใช้งานนโยบายนี้จะตั้งค่ารีจิสทรีคีย์ต่อไปนี้เป็น 0

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

ถ้าคุณไม่เห็นตัวเลือก ไฟล์ออนดีมานด์ ใน "การตั้งค่า" ตรวจสอบให้แน่ใจว่าชนิดการเริ่มต้น "โปรแกรมควบคุมตัวกรองไฟล์ระบบคลาวด์ของ Windows" ถูกตั้งค่าเป็น 2 (AUTO_START) การเปิดใช้งานฟีเจอร์นี้จะตั้งค่ารีจิสทรีคีย์ต่อไปนี้เป็น 2

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`