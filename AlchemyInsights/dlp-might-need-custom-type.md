---
title: DLP อาจจำเป็นต้องมีชนิดแบบกำหนดเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712203"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="ccecc-102">DLP อาจจำเป็นต้องมีชนิดแบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="ccecc-102">DLP might need a custom type</span></span>

<span data-ttu-id="ccecc-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="ccecc-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ccecc-104">**DLP อาจจำเป็นต้องมีชนิดข้อมูลแบบกำหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="ccecc-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="ccecc-105">ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและป้องกันข้อมูลที่สำคัญในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="ccecc-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="ccecc-106">ในบางสถานการณ์คุณอาจจำเป็นต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน **แบบกำหนดเอง** ของคุณเองเพื่อป้องกันข้อมูลขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ccecc-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="ccecc-107">ตัวอย่างเช่นองค์กรของคุณอาจจำเป็นต้องระบุและป้องกัน Id ของพนักงานหรือข้อมูลอื่นๆในรูปแบบบางอย่างที่เฉพาะเจาะจงสำหรับองค์กรของคุณ ถ้าเป็นเช่นนั้นให้ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="ccecc-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="ccecc-108">**การกำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="ccecc-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="ccecc-109">ถ้าชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในจะตอบสนองความต้องการของคุณได้ด้วยการปรับแต่งเพียงไม่กี่ครั้งคุณสามารถ [กำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)ได้</span><span class="sxs-lookup"><span data-stu-id="ccecc-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="ccecc-110">ตัวอย่างเช่นคุณสามารถเพิ่มหรือลบคำสำคัญหรือเพิ่มหรือเอาหลักฐานสนับสนุนออกเช่นวันที่หรือที่อยู่</span><span class="sxs-lookup"><span data-stu-id="ccecc-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="ccecc-111">**การสร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="ccecc-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="ccecc-112">แต่ถ้าคุณต้องการระบุและป้องกันชนิดของข้อมูลที่เป็นความลับที่แตกต่างกันทั้งหมดคุณสามารถ [สร้างชนิดข้อมูลที่สำคัญที่กำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) ใน UI ของศูนย์การปฏิบัติตามนโยบายการรักษาความปลอดภัย &</span><span class="sxs-lookup"><span data-stu-id="ccecc-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="ccecc-113">**การสร้างชนิดข้อมูลที่มีความสำคัญแบบกำหนดเองในการรักษาความปลอดภัย & ศูนย์การปฏิบัติตามนโยบายของ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="ccecc-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="ccecc-114">สุดท้ายถ้า UI ไม่มีตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถ[สร้างชนิดข้อมูลที่สำคัญที่กำหนดเองได้ในศูนย์การรักษาความปลอดภัย & การปฏิบัติตามนโยบายศูนย์การปฏิบัติตามนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="ccecc-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="ccecc-115">โดยเริ่มต้นด้วยไฟล์ XML คุณสามารถใช้ตัวเลือกทั้งหมดที่พร้อมใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="ccecc-115">By starting with an XML file, you can use every option available.</span></span>
