---
title: 126 ไม่พบข้อผิดพลาดการรับกล่องจดหมายใน OWA
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426681"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>พบข้อผิดพลาดไม่พบกล่องจดหมายใน Outlook บนเว็บใช่หรือไม่

ถ้าคุณใช้ Outlook บนเว็บ และไม่พบกล่องจดหมายจากข้อผิดพลาด บัญชีที่คุณใช้ในการเชื่อมต่อกับ Outlook บนเว็บจึงไม่มีสิทธิ์การใช้งาน Exchange Online ดังนั้นจึงไม่มีกล่องจดหมายที่เชื่อมโยงกับบัญชี ผู้ดูแลระบบของคุณสามารถกําหนดสิทธิการใช้งานให้กับบัญชีของคุณโดยปฏิบัติตามขั้นตอนเหล่านี้:

1. เปิด [ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/homepage)และ **ไปที่** ผู้ใช้ที่ใช้งานอยู่ภายใต้ส่วน ผู้ใช้ แล้วเลือกผู้ใช้ที่เห็นข้อผิดพลาด

2. ในหน้าผู้ใช้ที่เปิดขึ้น ให้ไปที่ส่วน สิทธิ์การใช้งานและ **แอป** เลือกค่าสถานที่ที่เหมาะสม และกําหนดสิทธิ์การใช้งานที่มี Exchange Online (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียด) เมื่อคุณเสร็จสิ้น ให้คลิก **บันทึกการเปลี่ยนแปลง**

ในบางกรณี ถ้าสิทธิ์การใช้งานถูกมอบหมายให้กับบัญชีผู้ใช้อยู่แล้ว การเอาออกและการมอบหมายสิทธิ์การใช้งานใหม่จะช่วยแก้ไขปัญหาและเตรียมใช้งานได้อย่างถูกต้องในระบบ ดังนี้ 

- ตรวจสอบเพื่อดูว่าการสมัครใช้งาน M365 Exchange Online (และอื่นๆ ถ้าคุณมี) เป็นการสมัครใช้งานปัจจุบันและยังไม่หมดอายุเมื่อเร็วๆ นี้

เมื่อคุณตรวจสอบให้แน่ใจว่าการสมัครใช้งานของคุณยังไม่หมดอายุและมีการมอบหมายสิทธิ์การใช้งานที่ถูกต้องให้กับบัญชีผู้ใช้ อาจใช้เวลาถึง 24 ชั่วโมงในการเตรียมสิทธิ์การใช้งาน ดังนั้นคุณอาจต้องรอให้ปัญหาของคุณแก้ไขปัญหา ดูข้อมูลเพิ่มเติมได้ที่ [กําหนดและจัดการ](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)สิทธิ์การใช้งาน