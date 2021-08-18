---
title: Modify Microsoft Edge by using data directory variables than hardcoded paths
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
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113435"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modify Microsoft Edge by using data directory variables than hardcoded paths

ตัวอย่างเช่น บนแท็บ Windowsข้อมูลโปรไฟล์ภายใต้ข้อมูลแอปพลิเคชันภายในของผู้ใช้แทนที่จะอยู่ในที่ตั้งเริ่มต้น ให้ตั้งค่านโยบาย **UserDataDir** เป็น **${local_app_data}\Edge\Profile** 

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[Microsoft Edgeตัวแปรไดเรกทอรีของข้อมูล](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)ผู้ใช้