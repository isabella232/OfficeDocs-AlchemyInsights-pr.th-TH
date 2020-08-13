---
title: แชนเนลส่วนตัว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005457"
---
# <a name="private-channels-in-microsoft-teams"></a>แชนเนลส่วนตัวในทีม Microsoft

แชนเนลส่วนตัวเป็นฟีเจอร์ใหม่ในทีม Microsoft โปรดสังเกตว่าไม่สามารถแปลงแชนเนลส่วนตัวจากแชนเนลมาตรฐานหรือกลับกันได้

สำหรับรายละเอียดเกี่ยวกับแชนเนลส่วนตัวเช่นข้อมูลเกี่ยวกับการ[สร้างแชนเนลส่วนตัวและการเป็นสมาชิก](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)และ[ไซต์ SharePoint ของแชนเนลส่วน](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)ตัวให้ดู[ที่แชนเนลส่วนตัวในทีม Microsoft](https://docs.microsoft.com/MicrosoftTeams/private-channels) 

**หมายเหตุ:** เนื่องจากการกำหนดค่าสำหรับการเก็บรักษาข้อความของแชนเนลส่วนตัวยังไม่ได้รับการสนับสนุนผู้เช่าที่มีนโยบายการเก็บข้อมูลที่เปิดใช้งานจะไม่มีแชนเนลส่วนตัวที่เปิดใช้งานตามค่าเริ่มต้น คุณสามารถเปิดใช้งานแชนเนลส่วนตัวในศูนย์การจัดการทีมได้ นอกจากนี้โปรดทราบว่าขณะที่การเก็บรักษาข้อความของแชนเนลส่วนตัวไม่ได้รับการสนับสนุนการเก็บข้อมูลของไฟล์ที่แชร์ในแชนเนลส่วนตัวจะได้รับการสนับสนุน

**จำเป็นต้องมีเจ้าของทีมใหม่ใช่หรือไม่**

ถ้าเจ้าของแชนเนลส่วนตัวของคุณคุณสามารถเพิ่มเจ้าของทีมใหม่ผ่านทางทีม Powershell ได้


- ไปที่[นี่](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)เพื่อติดตั้งทีม Powershell

ต่อไปนี้คือ cmdlet ที่คุณจำเป็นต้องมี:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับทีม Powershell ให้ดูที่[ภาพรวมของทีม powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)
