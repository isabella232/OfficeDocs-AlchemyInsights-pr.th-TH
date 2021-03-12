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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733868"
---
# <a name="11-call-recording"></a>การบันทึกการโทรแบบ 1:1

ผู้ดูแลระบบต้องจัดการทันทีเพื่ออนุญาตให้ผู้ใช้บันทึกการโทรแบบ 1:1 ได้ต่อไป
 
ตั้งแต่วันที่ 12 เมษายน 2021 เราจะเริ่มบังคับใช้ตัวเลือกนโยบายการโทรของ Teams ใหม่ *AllowCloudRecordingForCalls* 

ขณะนี้ความสามารถในการบันทึกการโทรแบบ 1:1 จะถูกควบคุมโดยตัวเลือก *AllowCloudRecording* ในนโยบายการประชุม Teams ถ้าผู้ใช้ของคุณได้รับอนุญาตให้บันทึกการประชุม Teams พวกเขาจะสามารถบันทึกการโทรแบบ 1:1 ได้

ถ้าคุณต้องการบล็อกผู้ใช้ทั้งหมดจากการบันทึกการโทรแบบ 1:1 คุณไม่ต้องการที่จะหยุดการใดๆ *AllowCloudRecordingForCalls* calling policy option will be $False by default.

การเปลี่ยนแปลงนี้อยู่ในโพสต์ของศูนย์ข้อความต่อไปนี้: (อัปเดต) บทนํานโยบายการบันทึกการโทรแบบ[1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)เมื่อต้องการตั้งค่าตัวเลือกนโยบายการโทรของ Teams คุณต้องใช้[Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**เมื่อต้องการเปิดใช้งานการบันทึกการโทรในการโทรแบบ 1:1 ให้** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**เมื่อต้องการปิดใช้งานการบันทึกการโทรในการโทรแบบ 1:1 ให้** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

