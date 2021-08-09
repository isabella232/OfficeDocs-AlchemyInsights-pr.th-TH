---
title: แนวคิดการรับรองความถูกต้องขั้นสูงที่ใช้กับMicrosoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934384"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>แนวคิดการรับรองความถูกต้องขั้นสูงที่ใช้กับMicrosoft Edge

ต่อไปนี้คือแนวคิดการรับรองความถูกต้องขั้นสูงที่สามารถใช้กับMicrosoft Edge:

**การรับรองความถูกต้องเชิงรุก**

เมื่อคุณเปิดใช้งานนโยบาย[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edgeจะพยายามรับรองความถูกต้องของผู้ใช้ที่ลงชื่อเข้าใช้ในเชิงรุกผ่านทางบริการของ Microsoftของคุณ ในช่วงเวลาที่สม่ากจะใช้บริการออนไลน์เพื่อตรวจสอบรายการอัปเดตที่มีการกําหนดค่าที่ควบคุมการรับรองความถูกต้องแบบโพรแอกทีฟ

สิทธิประโยชน์: การรับรองความถูกต้องในเชิงรุกจะเปิดใช้งานการรับรองความถูกต้องในบริการหลัก เช่น Office หน้าแท็บใหม่ นอกจากนี้ ถ้าคุณใช้ Bing เป็นโปรแกรมค้นหา การรับรองความถูกต้องแบบโพรแอกทีฟจะปรับปรุงประสิทธิภาพของแถบที่อยู่ และช่วยสร้างผลลัพธ์การค้นหาที่ปรับให้เหมาะกับความต้องการของธุรกิจของคุณ

**Windows Hello CredUI for NTLM Authentication**

ถ้าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) ไม่พร้อมใช้งานเมื่อเว็บไซต์พยายามลงชื่อเข้าใช้ผู้ใช้ผ่านกลไก NTLM หรือ Negotiate ฟีเจอร์นี้จะอนุญาตให้ผู้ใช้แชร์ข้อมูลรับรองความถูกต้องของระบบปฏิบัติการกับเว็บไซต์ และตอบสนองความท้าทายในการรับรองความถูกต้องโดยใช้ Windows Hello Cred UI โฟลว์การลงชื่อเข้าใช้นี้จะปรากฏเฉพาะในWindows 10 และเฉพาะผู้ใช้ที่ไม่ได้รับ SSO ระหว่างการท้าทาย NTLM หรือ Negotiate เท่านั้น

**ใช้รหัสผ่านที่บันทึกไว้เพื่อลงชื่อเข้าใช้โดยอัตโนมัติ**

ผู้ใช้ที่บันทึกรหัสผ่านใน Microsoft Edgeสามารถเปิดใช้งานการลงชื่อเข้าใช้อัตโนมัติไปยังเว็บไซต์ที่พวกเขาได้บันทึกข้อมูลอ้างอิงไว้ ผู้ใช้สามารถเปิดหรือปิดฟีเจอร์นี้ edge://settings/passwords และคุณสามารถกําหนดค่าใน [นโยบายตัวจัดการ](https://go.microsoft.com/fwlink/?linkid=2134622) รหัสผ่าน
