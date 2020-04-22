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
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704508"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="13aef-102">DLP อาจต้องการชนิดที่กําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="13aef-102">DLP might need a custom type</span></span>

<span data-ttu-id="13aef-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="13aef-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="13aef-104">**DLP อาจต้องการชนิดข้อมูลแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="13aef-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="13aef-105">ด้วยนโยบายการป้องกันข้อมูลสูญหาย (DLP) คุณจะสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="13aef-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="13aef-106">ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน**แบบกําหนดเอง**ของคุณเองเพื่อป้องกันข้อมูลองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="13aef-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="13aef-107">ตัวอย่างเช่น องค์กรของคุณอาจจําเป็นต้องระบุและป้องกันหมายเลขพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบเฉพาะกับองค์กรของคุณ ถ้าเป็นเช่นนั้น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="13aef-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="13aef-108">**กําหนดชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="13aef-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="13aef-109">หากชนิดข้อมูลที่สําคัญในตัวจะตอบสนองความต้องการของคุณมีเพียงการปรับแต่งไม่กี่คุณสามารถ[ปรับแต่งในตัวชนิดข้อมูลที่สําคัญ](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="13aef-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="13aef-110">ตัวอย่างเช่น คุณสามารถเพิ่มหรือนําคําหลักออก หรือเพิ่มหรือลบหลักฐานสนับสนุน เช่น วันที่หรือที่อยู่ออกได้</span><span class="sxs-lookup"><span data-stu-id="13aef-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="13aef-111">**สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="13aef-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="13aef-112">แต่ถ้าคุณต้องการระบุและป้องกันข้อมูลที่สําคัญชนิดอื่น &ทั้งหมด[create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="13aef-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="13aef-113">**สร้างชนิดข้อมูลที่สําคัญแบบกําหนดเองในการรักษาความปลอดภัย&ศูนย์ควบคุมการปฏิบัติตามกฎระเบียบ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="13aef-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="13aef-114">สุดท้ายถ้า UI ไม่ได้ให้ตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถสร้าง[ชนิดข้อมูลที่สําคัญที่กําหนดเองในการรักษาความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="13aef-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="13aef-115">โดยเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทั้งหมดที่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="13aef-115">By starting with an XML file, you can use every option available.</span></span>
