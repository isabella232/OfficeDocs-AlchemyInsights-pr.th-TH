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
ms.openlocfilehash: c6766c318f0058e66950dbd0ca2953b149579a5c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823374"
---
# <a name="accessing-files-in-microsoft-teams"></a>การเข้าถึงไฟล์ใน Microsoft Teams

ถ้าผู้ใช้มีปัญหาในการเข้าถึงไฟล์ใน Microsoft Teams ก่อนอื่นให้พิจารณาว่าไฟล์แนบมากับการสนทนาส่วนตัวหรือการสนทนาในแชนเนล แชนเนลทีมคือที่ที่ทุกคนในทีมสามารถสนทนากันอย่างเปิดกว้าง การแชทส่วนตัวจะมองเห็นได้เฉพาะบุคคลในการแชท (และไฟล์ที่คุณแชร์ในการแชทจะถูกเก็บไว้ใน OneDrive for Business)

เมื่อผู้ใช้แชร์ไฟล์ในการแชทส่วนตัว ไฟล์จะถูกเก็บไว้ใน OneDrive for Business ของผู้ใช้ที่แชร์ ถ้าผู้ใช้ถูกเพิ่มลงในการสนทนาส่วนตัวที่มีอยู่ พวกเขาจะไม่สามารถเข้าถึงไฟล์ได้ เว้นแต่เจ้าของเดิมจะแชร์ไฟล์อีกครั้ง    

**ในการสนทนาในแชนเนล:**

- [การแชร์ไฟล์ใน Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) จะยึดตามการตั้งค่าที่กําหนดค่าใน SharePoint หรือ OneDrive 
- ตรวจสอบ [การร่วมมือกันบนไฟล์กับ](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) ทีม ของคุณ เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับวิธีที่ Teams ช่วยให้องค์กรของคุณสามารถแชร์และร่วมมือกันบนไฟล์ได้ 
- หากสมาชิกในทีมใหม่พบความล่าช้าในการเข้าถึงไฟล์ โปรดรออย่างน้อย **4** ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุนเพื่อให้การลองแบบเสร็จสมบูรณ์ 

If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed. การเปลี่ยนชื่อไซต์ SharePoint และไลบรารีเอกสารของ Teams ยังไม่ได้รับการสนับสนุน เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดไซต์ทีมที่ใช้กับทีมนี้ แล้วเปลี่ยนชื่อไลบรารีกลับไปเป็น "เอกสารที่แชร์"