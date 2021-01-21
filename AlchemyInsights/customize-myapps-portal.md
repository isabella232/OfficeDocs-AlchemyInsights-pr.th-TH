---
title: กำหนแอปของฉันพอร์ทัลเอง
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7773"
- "9004350"
ms.openlocfilehash: e2d7cc165fce8be2e2c15d7d806917e309395d45
ms.sourcegitcommit: 688642f4ebc0f1c335e954e780bb9ec8893e2f3f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917161"
---
# <a name="customize-myapps-portal"></a>กำหนแอปของฉันพอร์ทัลเอง

1. ตัวเลือก **แอปล่าสุด** จะพร้อมใช้งานในขณะนี้ภายใต้ปุ่ม **แอปของฉัน Extention** ในพอร์ทัลแอปของฉัน
2. คุณสามารถเปลี่ยนชื่อชื่อของแต่ละคอลเลกชันที่สร้างขึ้นใน Azure Active Directory (AD) ได้แต่ไม่ใช่ชื่อของ **แอปทั้งหมด**
3. แอปพลิเคชัน Microsoft ไม่สามารถเอาออกจากคอลเลกชันแอปของฉันหรือเป็นส่วนหนึ่งของชุดคอลเลกชันที่แตกต่างกันได้
4. คุณสามารถปรับเปลี่ยนตัวเปิดใช้แอปได้ผ่านทาง Office portal แต่ไม่ใช่ผ่านทางพอร์ทัล MyApplications
5. สำหรับข้อมูลเกี่ยวกับวิธีการกำหนดโลโก้ของแอปพลิเคชันเองให้ดู[ที่ใช้โลโก้แบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#use-a-custom-logo)
6. เมื่อต้องการกำหนด URL สำหรับแอปพลิเคชันเองคุณสามารถลองทำตามขั้นตอนใดขั้นตอนหนึ่งต่อไปนี้:
    - การใช้ฟีเจอร์ **คอลเลกชัน** ของแอปพลิเคชันสำหรับองค์กร (ซึ่งจะทำให้คุณได้รับ URL เช่น: https://myapps.microosft.com/customAppName.com หรือบางสิ่งที่คล้ายกันโดยยึดตามการกำหนดค่าของคุณ)
    - ลองใช้แอปพลิเคชันแบบกำหนดเองในแอปพลิเคชันขององค์กรที่จะนำไปใช้กับ URL ที่เฉพาะเจาะจง
7. ให้ดู [ที่ตั้งค่าโฮมเพจที่กำหนดเองสำหรับการเผยแพร่แอปโดยใช้พร็อกซีแอปพลิเคชัน AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) สำหรับข้อมูลเกี่ยวกับวิธีการกำหนดค่าแอปเพื่อให้ผู้ใช้ไปยังโฮมเพจที่กำหนดเองโดยตรง
