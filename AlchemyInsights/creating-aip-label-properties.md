---
title: การสร้างนโยบายป้ายชื่อ AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569514"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="42d17-102">การสร้างนโยบายป้ายชื่อ AIP</span><span class="sxs-lookup"><span data-stu-id="42d17-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="42d17-103">ป้ายชื่อ Azure Data Protection(AIP) สามารถใช้กับข้อมูลเต็มรูปแบบที่องค์กรมักจะสร้างและจัดเก็บจากการจัดประเภทข้อมูลส่วนบุคคลต่ําสุดไปจนถึงการจําแนกข้อมูลลับสูงที่สุด</span><span class="sxs-lookup"><span data-stu-id="42d17-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="42d17-104">นโยบายการป้องกันข้อมูล azure นําไปใช้กับไคลเอนต์คลาสสิ Azure Protection(AIP) และไม่[AIP รวมการติดฉลากไคลเอนต์](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="42d17-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="42d17-105">คุณสามารถกําหนดค่าองค์ประกอบหลายองค์ประกอบในนโยบาย AIP รวมถึงตัวเลือกต่างๆ เช่น</span><span class="sxs-lookup"><span data-stu-id="42d17-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="42d17-106">ตัวเลือกที่ป้ายกํากับจะอนุญาตให้ผู้ดูแลระบบหรือผู้ใช้จัดประเภทและป้องกันเอกสารและอีเมล (ตัวเลือก)</span><span class="sxs-lookup"><span data-stu-id="42d17-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="42d17-107">ตัวเลือกในการบังคับใช้การจัดประเภทเมื่อผู้ใช้บันทึกเอกสารและส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="42d17-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="42d17-108">ตัวเลือกในการติดป้ายกํากับข้อความอีเมลโดยอัตโนมัติ ตามไฟล์แนบ</span><span class="sxs-lookup"><span data-stu-id="42d17-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="42d17-109">ตัวเลือกในการควบคุมว่าแถบการป้องกันข้อมูลจะแสดงในโปรแกรมประยุกต์ Office</span><span class="sxs-lookup"><span data-stu-id="42d17-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="42d17-110">สําหรับตัวเลือกเพิ่มเติมและข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการป้องกันข้อมูล Azure ให้ดูที่:[ภาพรวมของนโยบายการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/overview-policy)</span><span class="sxs-lookup"><span data-stu-id="42d17-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="42d17-111">สําหรับทรัพยากรที่เป็นประโยชน์อื่นๆ เกี่ยวกับนโยบาย AIP โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="42d17-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="42d17-112">บทช่วยสอน: กําหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่</span><span class="sxs-lookup"><span data-stu-id="42d17-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="42d17-113">การกําหนดค่านโยบายการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="42d17-114">สร้างและกําหนดค่าป้ายความละเอียดอ่อนและนโยบายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="42d17-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="42d17-115">คําแนะนําวิธีการสําหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="42d17-116">ตรวจทานเอกสารการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="42d17-117">ข้อกําหนดสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="42d17-118">บทช่วยสอนเริ่มต้นใช้งานอย่างย่อสําหรับการปกป้องข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="42d17-119">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="42d17-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)