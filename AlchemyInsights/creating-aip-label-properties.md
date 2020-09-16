---
title: การสร้างนโยบายป้ายชื่อ AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732194"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="802ff-102">การสร้างนโยบายป้ายชื่อ AIP</span><span class="sxs-lookup"><span data-stu-id="802ff-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="802ff-103">ป้ายชื่อการป้องกันข้อมูลของ Azure (AIP) สามารถใช้กับข้อมูลทั้งหมดที่องค์กรจะสร้างและจัดเก็บจากการจัดประเภทของข้อมูลส่วนบุคคลที่ต่ำที่สุดไปจนถึงการจัดประเภทของข้อมูลที่เป็นความลับสูงสุด</span><span class="sxs-lookup"><span data-stu-id="802ff-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="802ff-104">นโยบายการป้องกันข้อมูลของ azure จะนำไปใช้กับไคลเอ็นต์การป้องกันข้อมูล Azure (AIP) และไม่ใช่[ไคลเอ็นต์การติดฉลาก Aip Unified](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="802ff-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="802ff-105">คุณสามารถกำหนดค่าองค์ประกอบหลายองค์ประกอบในนโยบาย AIP รวมถึงตัวเลือกต่างๆเช่น:</span><span class="sxs-lookup"><span data-stu-id="802ff-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="802ff-106">ตัวเลือกสำหรับป้ายชื่อใดที่จะช่วยให้ผู้ดูแลระบบหรือการจัดประเภทผู้ใช้และการป้องกัน (ไม่จำเป็น) เอกสารและอีเมล</span><span class="sxs-lookup"><span data-stu-id="802ff-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="802ff-107">ตัวเลือกในการบังคับใช้การจัดประเภทเมื่อผู้ใช้บันทึกเอกสารและส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="802ff-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="802ff-108">ตัวเลือกในการป้ายชื่อข้อความอีเมลโดยยึดตามสิ่งที่แนบมาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="802ff-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="802ff-109">ตัวเลือกในการควบคุมว่าจะแสดงแถบการป้องกันข้อมูลในแอปพลิเคชัน Office หรือไม่</span><span class="sxs-lookup"><span data-stu-id="802ff-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="802ff-110">สำหรับตัวเลือกเพิ่มเติมและข้อมูลเกี่ยวกับนโยบายการป้องกันข้อมูลของ Azure ให้ดูที่:[ภาพรวมของนโยบายการป้องกันข้อมูลของ azure](https://docs.microsoft.com/azure/information-protection/overview-policy)</span><span class="sxs-lookup"><span data-stu-id="802ff-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="802ff-111">สำหรับแหล่งข้อมูลอื่นๆที่มีประโยชน์เกี่ยวกับนโยบายของ AIP ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="802ff-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="802ff-112">บทช่วยสอน: กำหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่</span><span class="sxs-lookup"><span data-stu-id="802ff-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="802ff-113">การกำหนดค่านโยบายการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="802ff-114">การสร้างและกำหนดค่าป้ายชื่อความลับและนโยบายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="802ff-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="802ff-115">เส้นบอกแนววิธีการสำหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="802ff-116">ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="802ff-117">ข้อกำหนดสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="802ff-118">บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="802ff-119">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="802ff-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)