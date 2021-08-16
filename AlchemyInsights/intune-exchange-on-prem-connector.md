---
title: Intun Exchange ตัวเชื่อมต่อภายในองค์กร
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013983"
---
# <a name="intune-exchange-on-premise-connector"></a>Intun Exchange ตัวเชื่อมต่อภายในองค์กร

For details of setting up the connector between Intun Exchange Exchange which is hosted on-premises please see the following documentation:

[ตั้งค่าตัวเชื่อมต่อภายในองค์กรแบบ Intun Exchangeใน Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**คำถามที่ถามบ่อย:**

Q: ฉันเห็นข้อผิดพลาด เช่น "Exchangeตัวเชื่อมต่อเอกสารไม่ได้รับการสนับสนุน" เมื่อพยายามExchangeตัวเชื่อมต่อ สาเหตุใดที่อาจเป็นสาเหตุ

A: บัญชีที่คุณใช้งานได้รับสิทธิ์การใช้งานอย่างเหมาะสม - บัญชีต้องมีสิทธิ์การใช้งาน Intun1 ที่ใช้งานอยู่

Q: สามารถมีตัวเชื่อมต่อแบบหลายExchangeได้หรือไม่

A: คุณสามารถตั้งค่าตัวเชื่อมต่ออุปกรณ์ได้เพียงหนึ่งExchangeต่อผู้เช่า Intuned ต่อExchangeองค์กรเท่านั้น ตัวเชื่อมต่อสามารถติดตั้งได้บนเซิร์ฟเวอร์เดียวในองค์กร Exchange แบบหลายเซิร์ฟเวอร์เท่านั้น

นอกจากนี้ คุณไม่สามารถกําหนดค่าตัวเชื่อมต่อไว้ทั้งExchangeภายในองค์กร และที่Exchange Onlineกําหนดค่าในผู้เช่าเดียวกันได้

Q: ตัวเชื่อมต่อสามารถใช้อาร์เรย์ CAS เป็นการเชื่อมต่อกับExchangeได้หรือไม่

A: การระบุอาร์เรย์ CAS ไม่ใช่การกําหนดค่าที่ได้รับการสนับสนุนในการตั้งค่าตัวเชื่อมต่อ ควรมีการระบุเซิร์ฟเวอร์เพียงเซิร์ฟเวอร์เดียวและควรใส่รหัสยากในไฟล์การกําหนดค่าตัวเชื่อมต่อซึ่งสามารถพบได้ใน

ข้อมูลโปรแกรม\microsoft\microsoft Intun on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

ค้นหารายการ ```<ExchangeWebServiceURL />``` ต่อไปนี้และแทนที่ URL ด้วยเซิร์ฟเวอร์ Exchange

**ตัวอย่าง:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

โปรดดูเอกสารประกอบต่อไปนี้เพื่อดูการแก้ไขปัญหาเพิ่มเติม:[แก้ไขปัญหาตัวเชื่อมต่อภายในองค์กร](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)Exchange

**การเปิดใช้งานการบันทึกแบบ Verbose Exchangeตัวเชื่อมต่อ**

1. เปิดไฟล์การExchangeกําหนดค่าการติดตามตัวเชื่อมต่อเพื่อแก้ไข  
ไฟล์จะอยู่ที่ : %ProgramData%\Microsoft\Windows Intun Exchange Connector\TracingConfiguration.xml  

**ตัวอย่าง:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. ค้นหา TraceSourceLine ด้วยคีย์ต่อไปนี้: OnPremisesExchangesConnectorService  
  
3. เปลี่ยนค่าโหนด SourceLevel จาก Information ActivityTracing (ค่าเริ่มต้น) เป็น Verbose ActivityTracing  

**ตัวอย่าง:**
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
4. เริ่มบริการการMicrosoft Intune Exchangeใหม่  
5. การซิงค์แบบเต็มรูปแบบในพอร์ทัล Intun1 จนกว่าจะเสร็จสิ้น แล้วเปลี่ยน XML กลับเป็น "Information ActivityTracing" แล้วเริ่มบริการการMicrosoft Intune Exchangeใหม่  
6. สถานที่ของบันทึกคือ: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`