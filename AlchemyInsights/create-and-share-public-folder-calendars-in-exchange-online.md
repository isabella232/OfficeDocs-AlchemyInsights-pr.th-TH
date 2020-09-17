---
title: สร้างและแชร์ปฏิทินของโฟลเดอร์สาธารณะใน Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804082"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a>สร้างและแชร์ปฏิทินของโฟลเดอร์สาธารณะใน Exchange Online

คุณสามารถสร้างปฏิทินในโฟลเดอร์สาธารณะได้จากไคลเอ็นต์ Outlook บนเดสก์ท็อปเท่านั้น ใช้ขั้นตอนเหล่านี้เพื่อตั้งค่าปฏิทินของโฟลเดอร์สาธารณะ:

1. ตรวจสอบให้แน่ใจว่ามีการจัดวางโฟลเดอร์สาธารณะใน Exchange Online สำหรับข้อมูลเพิ่มเติมให้ดู[ที่สร้างกล่องจดหมายโฟลเดอร์สาธารณะ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox) 

2. ตรวจสอบให้แน่ใจว่าคุณได้กำหนดสิทธิ์การเข้าถึงที่จำเป็นเพื่อสร้างโฟลเดอร์สาธารณะ สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของโฟลเดอร์สาธารณะสำหรับ Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server) 
  
3. ลงชื่อเข้าใช้ไคลเอ็นต์เดสก์ท็อปของ Outlook และตรวจสอบให้แน่ใจว่าคุณสามารถเข้าถึงการปรับใช้โฟลเดอร์สาธารณะของคุณได้

    ถ้าคุณกำลังมีปัญหาในการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ไคลเอ็นต์เดสก์ท็อปของ Outlook ให้ดูที่[ผู้ใช้ Exchange Online ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะได้โดยใช้ Outlook หรือ OWA](https://aka.ms/pfcte)

4. สร้างชนิดปฏิทินของโฟลเดอร์สาธารณะใหม่

โฟลเดอร์สาธารณะจะถูกแชร์กับผู้ใช้อื่นทั้งหมดตามค่าเริ่มต้น เจ้าของโฟลเดอร์สาธารณะสามารถเปลี่ยนแปลงสิทธิ์จากไคลเอ็นต์เดสก์ท็อปของ Outlook ได้ สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของโฟลเดอร์สาธารณะสำหรับ Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)

**หมายเหตุ:** ปฏิทินโฟลเดอร์สาธารณะได้รับการออกแบบมาเพื่อใช้ภายในองค์กรและไม่สามารถเผยแพร่บนอินเทอร์เน็ตได้ ใช้กล่องจดหมายที่แชร์ถ้าความตั้งใจของคุณคือการประกาศปฏิทินบนอินเทอร์เน็ต