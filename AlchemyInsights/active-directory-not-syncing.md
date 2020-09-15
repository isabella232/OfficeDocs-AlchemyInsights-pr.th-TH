---
title: ไดเรกทอรีที่ใช้งานอยู่ไม่ซิงค์
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697648"
---
# <a name="active-directory-not-syncing"></a>ไดเรกทอรีที่ใช้งานอยู่ไม่ซิงค์

ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลการดูแลระบบ Office ระบุว่า "การซิงค์ครั้งล่าสุดมากกว่า3วันที่แล้ว" อาจเป็นเพราะว่า AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ไม่เพียงพอที่จะทำการซิงโครไนซ์  

การติดตั้งใหม่ AADConnect โดยใช้การตั้งค่าแบบด่วนอาจแก้ไขปัญหาได้อย่างรวดเร็ว:

1. [ดาวน์โหลดเวอร์ชันล่าสุดของ AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [ทำตามคำแนะนำสำหรับการติดตั้งแบบด่วน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับบัญชีผู้ใช้บริการ AADConnect ให้ดูที่[AZURE AD Connect: บัญชีผู้ใช้และสิทธิ์](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
