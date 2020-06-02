---
title: DLP อาจต้องการชนิดที่กําหนดเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507533"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="3f4d5-102">DLP อาจต้องการชนิดที่กําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="3f4d5-102">DLP might need a custom type</span></span>

<span data-ttu-id="3f4d5-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3f4d5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="3f4d5-104">**DLP อาจต้องการชนิดข้อมูลที่กําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="3f4d5-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="3f4d5-105">ด้วยนโยบายการป้องกันข้อมูลสูญหาย (DLP) คุณสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="3f4d5-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="3f4d5-106">ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน**แบบกําหนดเอง**เพื่อปกป้องข้อมูลขององค์กร</span><span class="sxs-lookup"><span data-stu-id="3f4d5-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="3f4d5-107">ตัวอย่างเช่น องค์กรของคุณอาจจําเป็นต้องระบุและป้องกันรหัสพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบเฉพาะขององค์กรของคุณ ถ้าเป็นเช่นนั้น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="3f4d5-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="3f4d5-108">**กําหนดชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="3f4d5-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="3f4d5-109">หากข้อมูลที่สําคัญในตัวจะตอบสนองความต้องการของคุณมีเพียงการปรับแต่งไม่กี่, คุณสามารถกําหนด[ในตัวประเภทข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3f4d5-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="3f4d5-110">ตัวอย่างเช่น คุณสามารถเพิ่มหรือลบคําหลัก หรือเพิ่มหรือลบหลักฐานการสนับสนุน เช่น วันที่หรือที่อยู่</span><span class="sxs-lookup"><span data-stu-id="3f4d5-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="3f4d5-111">**สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="3f4d5-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="3f4d5-112">แต่ถ้าคุณต้องการระบุและป้องกันข้อมูลที่สําคัญชนิดอื่น &ทั้งหมด[create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="3f4d5-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="3f4d5-113">**สร้างชนิดข้อมูลที่สําคัญแบบกําหนดเองในความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="3f4d5-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="3f4d5-114">สุดท้ายถ้า UI ไม่ได้มีตัวเลือกทั้งหมดที่คุณต้องการ[คุณสามารถสร้างชนิดข้อมูลที่สําคัญที่กําหนดเองในการรักษาความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3f4d5-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="3f4d5-115">โดยเริ่มต้นด้วยไฟล์ XML คุณสามารถใช้ทุกตัวเลือกที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="3f4d5-115">By starting with an XML file, you can use every option available.</span></span>
