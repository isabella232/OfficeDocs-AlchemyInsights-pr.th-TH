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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="ea582-102">ตัวเชื่อมต่อการแลกเปลี่ยนในองค์กรของ Intune</span><span class="sxs-lookup"><span data-stu-id="ea582-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="ea582-103">สำหรับรายละเอียดเกี่ยวกับการตั้งค่าตัวเชื่อมต่อระหว่าง Intune และ Exchange ที่โฮสต์ภายในองค์กรโปรดดูเอกสารต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ea582-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="ea582-104">ตั้งค่าตัวเชื่อมต่อ Exchange ภายในองค์กรของ Intune ใน Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="ea582-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="ea582-105">**คำถามที่ถามบ่อย:**</span><span class="sxs-lookup"><span data-stu-id="ea582-105">**FAQ:**</span></span>

<span data-ttu-id="ea582-106">Q: ฉันเห็นข้อผิดพลาดเช่น "เวอร์ชันของตัวเชื่อมต่อ Exchange ไม่ได้รับการสนับสนุน" เมื่อพยายามตั้งค่าตัวเชื่อมต่อ Exchange</span><span class="sxs-lookup"><span data-stu-id="ea582-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="ea582-107">สาเหตุคืออะไร</span><span class="sxs-lookup"><span data-stu-id="ea582-107">What could be the cause?</span></span>

<span data-ttu-id="ea582-108">A: บัญชีผู้ใช้ที่คุณกำลังใช้ได้รับสิทธิ์การใช้งานอย่างเหมาะสม-จะต้องมีสิทธิ์การใช้งาน Intune ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="ea582-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="ea582-109">Q: สามารถมีตัวเชื่อมต่อ Exchange ได้หลายตัวหรือไม่</span><span class="sxs-lookup"><span data-stu-id="ea582-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="ea582-110">A: คุณสามารถตั้งค่าตัวเชื่อมต่อ Exchange หนึ่งรายการต่อผู้เช่า Intune ต่อองค์กร Exchange เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="ea582-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="ea582-111">สามารถติดตั้งตัวเชื่อมต่อบนเซิร์ฟเวอร์เดียวในองค์กร exchange server หลายองค์กรเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="ea582-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="ea582-112">นอกจากนี้คุณไม่สามารถมีตัวเชื่อมต่อที่กำหนดค่าสำหรับทั้ง Exchange ภายในองค์กรและ Exchange Online ที่กำหนดค่าไว้ในผู้เช่าเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="ea582-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="ea582-113">Q: ตัวเชื่อมต่อสามารถใช้อาร์เรย์ CAS เป็นการเชื่อมต่อกับ Exchange ได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="ea582-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="ea582-114">A: การระบุอาร์เรย์ CAS ไม่ใช่การกำหนดค่าที่ได้รับการสนับสนุนในการตั้งค่าตัวเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="ea582-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="ea582-115">เฉพาะเซิร์ฟเวอร์เดียวเท่านั้นที่ควรระบุและควรจะ hardcoded ในไฟล์การกำหนดค่าตัวเชื่อมต่อที่สามารถพบได้ใน</span><span class="sxs-lookup"><span data-stu-id="ea582-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="ea582-116">โปรแกรม data\microsoft\microsoft Intune บนตัวเชื่อมต่อ Exchange ที่มีอยู่ \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="ea582-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="ea582-117">ค้นหารายการต่อไปนี้ ```<ExchangeWebServiceURL />``` และแทนที่ URL ด้วย exchange server</span><span class="sxs-lookup"><span data-stu-id="ea582-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="ea582-118">**ตัวอย่าง**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="ea582-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="ea582-119">โปรดดูเอกสารประกอบต่อไปนี้สำหรับการแก้ไขปัญหาเพิ่มเติม: [แก้ไขปัญหาตัวเชื่อมต่อ Exchange ภายในองค์กรของ Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="ea582-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="ea582-120">**การเปิดใช้งานการบันทึก Verbose สำหรับตัวเชื่อมต่อ Exchange**</span><span class="sxs-lookup"><span data-stu-id="ea582-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="ea582-121">เปิดไฟล์การกำหนดค่าการติดตามตัวเชื่อมต่อของ Exchange สำหรับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="ea582-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="ea582-122">ไฟล์จะอยู่ที่:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="ea582-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="ea582-123">**ตัวอย่าง**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="ea582-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="ea582-124">ค้นหา TraceSourceLine ด้วยคีย์ต่อไปนี้: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="ea582-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="ea582-125">เปลี่ยนค่าโหน SourceLevel จาก ActivityTracing ข้อมูล (ค่าเริ่มต้น) เป็น Verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="ea582-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="ea582-126">**ตัวอย่าง**</span><span class="sxs-lookup"><span data-stu-id="ea582-126">**Example:**</span></span>
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
4. <span data-ttu-id="ea582-127">เริ่มบริการ Microsoft Intune Exchange ของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea582-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="ea582-128">การซิงค์แบบเต็มในพอร์ทัล Intune จนกว่าจะเสร็จสิ้นแล้วเปลี่ยน XML กลับเป็น "ข้อมูล ActivityTracing" แล้วเริ่มบริการ Microsoft Intune Exchange ของ Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ea582-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="ea582-129">ตำแหน่งที่ตั้งของไฟล์บันทึกคือ: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="ea582-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>