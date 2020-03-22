---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891768"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะ

ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทํางานสําหรับผู้ใช้บางราย ให้ลองทําดังต่อไปนี้

เชื่อมต่อกับ POWERShell EXO และกําหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox ในบัญชีผู้ใช้ปัญหาให้ตรงกับพารามิเตอร์ในบัญชีผู้ใช้ที่ทํางาน

ตัว อย่าง เช่น:

รับกล่องจดหมายทํางานผู้ใช้ | ฟุตเริ่มต้นโฟลเดอร์สาธารณะกล่องจดหมาย, ที่มีประสิทธิภาพสาธารณะโฟลเดอร์กล่องจดหมาย

ตั้งค่ากล่องจดหมายปัญหาผู้ใช้ -DefaultPublicFolderกล่องจดหมาย\<ค่าจากคําสั่งก่อนหน้านี้>

รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล

ถ้าปัญหายังคงอยู่ โปรดทําตามขั้นตอน[นี้เพื่อ](https://aka.ms/pfcte)แก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook