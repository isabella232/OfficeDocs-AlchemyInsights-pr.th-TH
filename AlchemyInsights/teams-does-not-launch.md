---
title: Teamsไม่เปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329345"
---
# <a name="teams-doesnt-launch"></a>Teamsไม่เปิดใช้งาน

ถ้าคุณพยายามเปิดMicrosoft Teamsแต่ไม่เปิดใช้ ให้ลองวิธีต่อไปนี้:

1. เรียกดู **%appdata%\Microsoft\Teams**
1. ลบเนื้อหาของโฟลเดอร์
1. รีสตาร์ตคอมพิวเตอร์ และลองTeamsอีกครั้ง

คุณอาจต้องติดตั้งซอฟต์แวร์Teamsอีกครั้ง เมื่อต้องการติดตั้งอีกครั้ง:

1. ถอนการติดตั้ง Teamsโดยใช้ แผงควบคุม
1. เรียกดู **%appdata%\Microsoft\Teams\Application Cache**
1. ลบเนื้อหาของโฟลเดอร์
1. เรียกดู **%appdata%\Microsoft\teams\Cache**
1. ลบเนื้อหาของโฟลเดอร์
1. รีสตาร์ตคอมพิวเตอร์ จากนั้นดาวน์โหลดและติดตั้งTeamsใหม่

ถ้าคุณต้องการเรียกใช้การวินิจฉัยในผู้เช่าของคุณของผู้ใช้ที่ระบุที่ไม่สามารถลงชื่อเข้าใช้ได้ ให้เริ่มการค้นหาใหม่ด้วยคีย์เวิร์ด **TeamsUserUnableToSignIn** และปฏิบัติตามพร้อมท์