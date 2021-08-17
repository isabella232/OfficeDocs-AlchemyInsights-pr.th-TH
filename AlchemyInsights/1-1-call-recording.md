---
title: การบันทึกการโทรแบบ 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886158"
---
# <a name="11-call-recording"></a>การบันทึกการโทรแบบ 1:1

ถ้า **ปุ่ม เริ่ม** การบันทึก เป็นสีเทาในการโทรแบบ 1:1 คุณต้องเปลี่ยนการตั้งค่านโยบายของผู้ใช้ที่ได้รับผลกระทบ เมื่อต้องการตรวจสอบการตั้งค่านโยบาย ให้เรียกใช้การวินิจฉัยของผู้ใช้ที่มีผลกระทบโดยการพิมพ์ **Diag: Teams 1:1 ตาม** ด้านบน     

ตั้งแต่วันที่ 31 พฤษภาคม 2021 เราจะเริ่มบังคับใช้นโยบายการโทรTeams *AllowCloudRecordingForCalls* ใหม่ ก่อนการเปลี่ยนแปลงนี้ การบันทึกการโทร 1:1 จะถูกควบคุมโดย *AllowCloudRecording Teams* นโยบายการประชุม การเปลี่ยนแปลงนี้อยู่ในโพสต์ของศูนย์ข้อความ: [(อัปเดตแล้ว) 1:1 บทนํานโยบายการบันทึก](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)การโทร  

*AllowCloudRecordingForCalls*   ตัวเลือกนโยบายการโทรถูกตั้งค่า **$False** ตามค่าเริ่มต้น ถ้าคุณต้องการบล็อกผู้ใช้ทั้งหมดไม่ให้บันทึกการโทรแบบ 1:1 คุณไม่ต้จะต้องการใดๆ  

เมื่อต้องการเปิดใช้งานการบันทึกการโทรให้กับผู้ใช้ทั้งหมดในการโทรแบบ 1:1 [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)เพื่อเรียกใช้ cmdlet ต่อไปนี้: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

อีกวิธีหนึ่งคือ คุณสามารถสร้างนโยบายใหม่และตั้งค่า **-AllowCloudRecordingForCalls** **$true** และกําหนดนโยบายนั้นให้กับผู้ใช้ของคุณ 

ดูข้อมูลเพิ่มเติมที่[1:1 การควบคุมนโยบายการบันทึกการโทร (เกือบเสร็จแล้ว!) ที่นี่](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
