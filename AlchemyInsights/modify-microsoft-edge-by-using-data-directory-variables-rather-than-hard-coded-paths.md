---
title: ปรับเปลี่ยนMicrosoft Edgeโดยใช้ตัวแปรไดเรกทอรีข้อมูลแทนเส้นทางที่ตายตัว
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992310"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>ปรับเปลี่ยนMicrosoft Edgeโดยใช้ตัวแปรไดเรกทอรีข้อมูลแทนเส้นทางที่ตายตัว

ตัวอย่างเช่น บนแท็บ Windowsข้อมูลโปรไฟล์ภายใต้ข้อมูลแอปพลิเคชันภายในของผู้ใช้แทนที่จะอยู่ในที่ตั้งเริ่มต้น ให้ตั้งค่านโยบาย *UserDataDir* เป็น **${local_app_data}\Edge\Profile**

For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).