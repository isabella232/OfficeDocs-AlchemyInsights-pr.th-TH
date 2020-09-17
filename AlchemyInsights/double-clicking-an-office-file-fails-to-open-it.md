---
title: การดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812098"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>การดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์

หลังจากดับเบิลคลิกที่ไฟล์ Office คุณอาจเห็นโปรแกรมเปิดแต่ไฟล์ตัวเองไม่เปิดขึ้น หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งคำสั่งไปยังโปรแกรม" มีหลายสาเหตุสำหรับสิ่งนี้แต่มีวิธีแก้ไขปัญหาที่พบมากที่สุดสองวิธีดังนี้

- จากภายใน Excel ให้ตรวจสอบให้แน่ใจว่าตัวเลือก DDE ไม่ได้ถูกยกเลิก คุณสามารถค้นหาตัวเลือกได้โดยการสร้างเวิร์กบุ๊กใหม่แล้วเลือก**ตัวเลือก > ไฟล์ > ขั้นสูง** ในส่วน**ทั่วไป**ให้ยกเลิกการเลือก**ละเว้นแอปพลิเคชันอื่นที่ใช้การแลกเปลี่ยนข้อมูลแบบไดนามิก (DDE)**

- เรียกใช้การซ่อมแซมแบบออนไลน์เพื่อคืนค่าการตั้งค่าเริ่มต้น คลิกปุ่มเริ่มของ Windows และค้นหา "แผงควบคุม" เปิด**แผงควบคุม**และไปที่**โปรแกรม > โปรแกรมและฟีเจอร์** จากนั้นคลิกขวาที่**Microsoft Office [เวอร์ชัน]** แล้วเลือก**เปลี่ยน > การซ่อมแซมแบบออนไลน์**

ถ้าไม่มีวิธีแก้ไขปัญหาเหล่านี้คุณสามารถดูรายการของโซลูชันที่สมบูรณ์มากขึ้นได้ในบทความสนับสนุนการ[ดับเบิลคลิกที่ไฟล์ Office ล้มเหลวในการเปิดไฟล์](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
