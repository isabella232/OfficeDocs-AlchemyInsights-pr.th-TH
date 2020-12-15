---
title: ปรับเปลี่ยน Microsoft Edge โดยใช้ตัวแปรไดเรกทอรีข้อมูลแทนที่จะเป็นเส้นทาง hardcoded
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679154"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>ปรับเปลี่ยน Microsoft Edge โดยใช้ตัวแปรไดเรกทอรีข้อมูลแทนที่จะเป็นเส้นทาง hardcoded

ตัวอย่างเช่นบน Windows เมื่อต้องการจัดเก็บข้อมูลโปรไฟล์ภายใต้ข้อมูลแอปพลิเคชันภายในของผู้ใช้แทนที่จะเป็นตำแหน่งที่ตั้งเริ่มต้นให้ตั้งค่านโยบาย **UserDataDir** เป็น **$ {local_app_data} \Edge\Profile** 

เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[สร้างตัวแปรไดเรกทอรีข้อมูลของผู้ใช้ Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)