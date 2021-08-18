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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091109"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>แก้ไขปัญหาการติดตั้ง MDATP บน Mac

ถ้าการติดตั้งด้วยตนเองล้มเหลว **หน้า สรุป** ของตัวช่วยสร้างการติดตั้งจะแสดงข้อผิดพลาดต่อไปนี้:

"มีข้อผิดพลาดเกิดขึ้นในระหว่างการติดตั้ง ตัวติดตั้งพบข้อผิดพลาดที่เป็นสาเหตุให้การติดตั้งล้มเหลว ติดต่อผู้ผลิตซอฟต์แวร์เพื่อขอความช่วยเหลือ"

ในการปรับใช้ MDM หน้าจะแสดงการติดตั้งทั่วไปล้มเหลวเช่นกัน

แม้ว่าเราจะไม่แสดงข้อผิดพลาดที่แน่นอนต่อผู้ใช้ แต่เราเก็บไฟล์บันทึกที่มีความคืบหน้าการติดตั้งไว้ใน **/Library/Logs/Microsoft/mdatp/install.log** เซสชันการติดตั้งแต่ละรายการจะผนวกเข้ากับไฟล์บันทึกนี้ เมื่อต้องการแสดงผลเซสชันการติดตั้งล่าสุด `sed` เท่านั้น ให้ใช้

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[แก้ไขปัญหาการติดตั้งของ Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615)
