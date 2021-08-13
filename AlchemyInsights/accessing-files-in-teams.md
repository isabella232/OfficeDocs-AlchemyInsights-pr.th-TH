---
title: การเข้าถึงไฟล์ใน Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2675"
- "9000710"
ms.openlocfilehash: 1c2e787bb6be02faea59adbe8b5236897789637696db0e9c48a5d13e9b9a92c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938606"
---
# <a name="accessing-files-in-microsoft-teams"></a>การเข้าถึงไฟล์ใน Microsoft Teams

ถ้าผู้ใช้มีปัญหาในการเข้าถึงไฟล์ในMicrosoft Teams ก่อนอื่นให้ระบุว่าไฟล์แนบมากับการสนทนาส่วนตัวหรือการสนทนาในแชนเนล แชนเนลทีมคือที่ที่ทุกคนในทีมสามารถสนทนากันอย่างเปิดกว้าง การแชทส่วนตัวจะมองเห็นได้เฉพาะบุคคลในการแชทเท่านั้น (และไฟล์ที่คุณแชร์ในการแชทจะถูกเก็บไว้ในOneDrive for Business)

When users share files in private chats, the file is stored on the sharing user's OneDrive for Business. ถ้าผู้ใช้ถูกเพิ่มลงในการสนทนาส่วนตัวที่มีอยู่ พวกเขาจะไม่สามารถเข้าถึงไฟล์ได้ เว้นแต่เจ้าของเดิมจะแชร์ไฟล์อีกครั้ง    

**ในการสนทนาในแชนเนล:**

- [การแชร์ไฟล์Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams)จะขึ้นอยู่กับการตั้งค่าที่กําหนดค่าSharePointหรือOneDrive 
- ตรวจสอบ[การร่วมมือกันบนไฟล์](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae)กับทีมของคุณ เพื่อเรียนรู้เพTeamsวิธีที่องค์กรของคุณสามารถแชร์และร่วมมือกันบนไฟล์ได้ 
- หากสมาชิกในทีมใหม่พบความล่าช้าในการเข้าถึงไฟล์ โปรดรออย่างน้อย **4** ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุนเพื่อให้การลองแบบเสร็จสมบูรณ์ 

ถ้าผู้ใช้สามารถเข้าถึงไฟล์ผ่านทางแท็บ ไฟล์ ในแชนเนลทีม และคุณได้รับข้อผิดพลาด "ไฟล์เหล่านี้ไม่พร้อมใช้งานอีกต่อไป" ให้ตรวจสอบเพื่อดูว่าไซต์ SharePoint หรือไลบรารีเอกสารถูกเปลี่ยนชื่อแล้วหรือไม่ การSharePointไซต์และไลบรารีเอกสารTeamsไซต์ของคุณยังไม่ได้รับการสนับสนุน เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดไซต์ทีมที่ใช้กับทีมนี้ แล้วเปลี่ยนชื่อไลบรารีกลับไปเป็น "เอกสารที่แชร์"