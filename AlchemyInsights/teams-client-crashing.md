---
title: ลูกค้าทีมล้มเหลว?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030669"
---
# <a name="teams-client-crashing"></a>ลูกค้าทีมล้มเหลว?

หากไคลเอ็นต์ Teams ของคุณหยุดทํางาน ให้ลองทําดังต่อไปนี้

- ถ้าคุณกําลังใช้แอปทีมบนเดสก์ท็อป ให้ตรวจสอบ[ให้แน่ใจว่าแอปได้รับการอัปเดตอย่างสมบูรณ์](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)แล้ว

- ตรวจสอบให้แน่ใจว่าสามารถเข้าถึง[URL ของ Office 365 และช่วงที่อยู่](https://docs.microsoft.com/microsoftteams/connectivity-issues)ทั้งหมดได้

- เข้าสู่ระบบด้วยบัญชีผู้ดูแลระบบและตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://docs.microsoft.com/office365/enterprise/view-service-health)เพื่อตรวจสอบว่าไม่มีการเสื่อมสภาพหรือการบริการ

 - ขั้นตอนสุดท้าย คุณสามารถพยายามล้างแคชของไคลเอ็นต์ Teams ของคุณ:

    1.  ออกจากไคลเอ็นต์เดสก์ท็อปทีม Microsoft อย่างสมบูรณ์ คุณสามารถคลิกขวาที่**ทีม**จากถาดไอคอน และคลิก**ออก**หรือเรียกใช้ตัวจัดการงาน และฆ่ากระบวนการทั้งหมด

    2.  ไปที่ File Explorer แล้วพิมพ์ข้อมูล %Microsoft\ทีม

    3.  เมื่ออยู่ในไดเรกทอรีคุณจะเห็นโฟลเดอร์ต่อไปนี้:

         - จากภายใน**แคชแอพลิเคชัน**ไปที่แคชและลบไฟล์ใด ๆ ในแคชที่ตั้ง: %appdata%\Microsoft \ทีมงาน \ แคชใบสมัคร

        - จาก**ภายในBlob_storage**ลบแฟ้มทั้งหมด: %appdata%\Microsoft\ทีม\blob_storage

        - จากภายใน**แคช**ลบไฟล์ทั้งหมด: %appdata%\ทีม\แคช

        - จาก**ภายในฐานข้อมูล**ลบแฟ้มทั้งหมด: %appdata%\Microsoft\ทีม\ฐานข้อมูล

        - จากภายใน**GPUCache**ลบไฟล์ทั้งหมด: %appdata%\ทีม\GPUcache

        - จากภายใน**ดัชนี DB**ให้ลบแฟ้ม .db: %appdata%\Microsoft\ทีม\ทําดัชนีDB

        - จาก**ภายในที่เก็บภายใน**ให้ลบแฟ้มทั้งหมด: %appdata%\Microsoft\teams\ที่เก็บข้อมูลภายในเครื่อง

        - สุดท้ายจากภายใน**tmp**ลบไฟล์ใด ๆ: %appdata%\ทีม\ทีม\tmp

    4. รีสตาร์ทไคลเอนต์ Teams ของคุณ
