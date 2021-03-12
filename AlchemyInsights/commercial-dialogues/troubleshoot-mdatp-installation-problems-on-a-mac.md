---
title: แก้ไขปัญหาการติดตั้ง MDATP บน Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749766"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>แก้ไขปัญหาการติดตั้ง MDATP บน Mac

ถ้าการติดตั้งด้วยตนเองล้มเหลว **หน้าสรุป** ของตัวช่วยสร้างการติดตั้งจะแสดงข้อผิดพลาดต่อไปนี้:

"มีข้อผิดพลาดเกิดขึ้นในระหว่างการติดตั้ง ตัวติดตั้งพบข้อผิดพลาดที่เป็นสาเหตุให้การติดตั้งล้มเหลว ติดต่อผู้ผลิตซอฟต์แวร์เพื่อขอความช่วยเหลือ"

ในการปรับใช้ MDM หน้าจะแสดงการติดตั้งทั่วไปล้มเหลวเช่นกัน

แม้ว่าเราจะไม่แสดงข้อผิดพลาดที่แน่นอนต่อผู้ใช้ แต่เราเก็บไฟล์บันทึกที่มีความคืบหน้าการติดตั้งไว้ใน **/Library/Logs/Microsoft/mdatp/install.log** เซสชันการติดตั้งแต่ละรายการจะผนวกเข้ากับไฟล์บันทึกนี้ เมื่อต้องการแสดงผลเซสชันการติดตั้งล่าสุด `sed` เท่านั้น ให้ใช้

หากต้องการเรียนรู้เพิ่มเติม โปรดดู[การแก้ไขปัญหาการติดตั้งของ Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615)
