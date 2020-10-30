---
title: ตัวเชื่อมต่อการแลกเปลี่ยนในองค์กรของ Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808139"
---
# <a name="intune-exchange-on-premise-connector"></a>ตัวเชื่อมต่อการแลกเปลี่ยนในองค์กรของ Intune

สำหรับรายละเอียดเกี่ยวกับการตั้งค่าตัวเชื่อมต่อระหว่าง Intune และ Exchange ที่โฮสต์ภายในองค์กรโปรดดูเอกสารต่อไปนี้:

[ตั้งค่าตัวเชื่อมต่อ Exchange ภายในองค์กรของ Intune ใน Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**คำถามที่ถามบ่อย:**

Q: ฉันเห็นข้อผิดพลาดเช่น "เวอร์ชันของตัวเชื่อมต่อ Exchange ไม่ได้รับการสนับสนุน" เมื่อพยายามตั้งค่าตัวเชื่อมต่อ Exchange สาเหตุคืออะไร

A: บัญชีผู้ใช้ที่คุณกำลังใช้ได้รับสิทธิ์การใช้งานอย่างเหมาะสม-จะต้องมีสิทธิ์การใช้งาน Intune ที่ใช้งานอยู่

Q: สามารถมีตัวเชื่อมต่อ Exchange ได้หลายตัวหรือไม่

A: คุณสามารถตั้งค่าตัวเชื่อมต่อ Exchange หนึ่งรายการต่อผู้เช่า Intune ต่อองค์กร Exchange เท่านั้น สามารถติดตั้งตัวเชื่อมต่อบนเซิร์ฟเวอร์เดียวในองค์กร exchange server หลายองค์กรเท่านั้น

นอกจากนี้คุณไม่สามารถมีตัวเชื่อมต่อที่กำหนดค่าสำหรับทั้ง Exchange ภายในองค์กรและ Exchange Online ที่กำหนดค่าไว้ในผู้เช่าเดียวกัน

Q: ตัวเชื่อมต่อสามารถใช้อาร์เรย์ CAS เป็นการเชื่อมต่อกับ Exchange ได้หรือไม่

A: การระบุอาร์เรย์ CAS ไม่ใช่การกำหนดค่าที่ได้รับการสนับสนุนในการตั้งค่าตัวเชื่อมต่อ เฉพาะเซิร์ฟเวอร์เดียวเท่านั้นที่ควรระบุและควรจะ hardcoded ในไฟล์การกำหนดค่าตัวเชื่อมต่อที่สามารถพบได้ใน

โปรแกรม data\microsoft\microsoft Intune บนตัวเชื่อมต่อ Exchange ที่มีอยู่ \ OnpremiseExchangeConnectorServiceConfiguration.xml

ค้นหารายการต่อไปนี้ ```<ExchangeWebServiceURL />``` และแทนที่ URL ด้วย exchange server

**ตัวอย่าง**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

โปรดดูเอกสารประกอบต่อไปนี้สำหรับการแก้ไขปัญหาเพิ่มเติม: [แก้ไขปัญหาตัวเชื่อมต่อ Exchange ภายในองค์กรของ Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**การเปิดใช้งานการบันทึก Verbose สำหรับตัวเชื่อมต่อ Exchange**

1. เปิดไฟล์การกำหนดค่าการติดตามตัวเชื่อมต่อของ Exchange สำหรับการแก้ไข  
ไฟล์จะอยู่ที่:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**ตัวอย่าง**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. ค้นหา TraceSourceLine ด้วยคีย์ต่อไปนี้: OnPremisesExchangeConnectorService  
  
3. เปลี่ยนค่าโหน SourceLevel จาก ActivityTracing ข้อมูล (ค่าเริ่มต้น) เป็น Verbose ActivityTracing  

**ตัวอย่าง**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. เริ่มบริการ Microsoft Intune Exchange ของ Microsoft  
5. การซิงค์แบบเต็มในพอร์ทัล Intune จนกว่าจะเสร็จสิ้นแล้วเปลี่ยน XML กลับเป็น "ข้อมูล ActivityTracing" แล้วเริ่มบริการ Microsoft Intune Exchange ของ Microsoft Intune  
6. ตำแหน่งที่ตั้งของไฟล์บันทึกคือ: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`