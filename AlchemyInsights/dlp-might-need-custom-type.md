---
title: DLP อาจต้องการชนิดที่กําหนดเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932677"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="aa1e1-102">DLP อาจต้องการชนิดที่กําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="aa1e1-102">DLP might need a custom type</span></span>

<span data-ttu-id="aa1e1-103">**สําคัญ**: SharePoint แบบออนไลน์และลูกค้า OneDrive เรียกใช้โปรแกรมประยุกต์ที่สําคัญทางธุรกิจกับบริการที่ทํางานในพื้นหลัง</span><span class="sxs-lookup"><span data-stu-id="aa1e1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="aa1e1-104">การป้องกันข้อมูลสูญหาย (DLP) และโซลูชันการสํารองข้อมูล</span><span class="sxs-lookup"><span data-stu-id="aa1e1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="aa1e1-105">ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่าบริการ SharePoint Online และ OneDrive ยังคงพร้อมใช้งานและเชื่อถือได้สําหรับผู้ใช้ของคุณซึ่งขึ้นอยู่กับบริการมากกว่าที่เคยในสถานการณ์การทํางานระยะไกล</span><span class="sxs-lookup"><span data-stu-id="aa1e1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="aa1e1-106">ในการสนับสนุนของวัตถุประสงค์นี้เราได้ดําเนินการจํากัดการควบคุมที่เข้มงวดมากขึ้นในปพลิเคชันพื้นหลัง (การย้ายถิ่น, DLP และโซลูชั่นการสํารองข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="aa1e1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="aa1e1-107">คุณควรคาดหวังว่าแอปเหล่านี้จะมีปริมาณงานที่จํากัดมากในช่วงเวลาเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="aa1e1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="aa1e1-108">อย่างไรก็ตามในช่วงเย็นและวันหยุดสุดสัปดาห์สําหรับภูมิภาคบริการจะพร้อมที่จะดําเนินการปริมาณการร้องขอจากแอปพื้นหลังที่สูงกว่าอย่างมีนัยสําคัญ</span><span class="sxs-lookup"><span data-stu-id="aa1e1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="aa1e1-109">**DLP อาจต้องการชนิดข้อมูลแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="aa1e1-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="aa1e1-110">ด้วยนโยบายการป้องกันข้อมูลสูญหาย (DLP) คุณจะสามารถระบุและปกป้องข้อมูลที่ละเอียดอ่อนในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="aa1e1-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="aa1e1-111">ในบางสถานการณ์ คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน**แบบกําหนดเอง**ของคุณเองเพื่อป้องกันข้อมูลองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="aa1e1-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="aa1e1-112">ตัวอย่างเช่น องค์กรของคุณอาจจําเป็นต้องระบุและป้องกันหมายเลขพนักงานหรือข้อมูลอื่นๆ ในบางรูปแบบเฉพาะกับองค์กรของคุณ ถ้าเป็นเช่นนั้น ให้ดูบทความต่อไปนี้สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="aa1e1-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="aa1e1-113">**กําหนดชนิดข้อมูลที่ละเอียดอ่อนที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="aa1e1-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="aa1e1-114">หากชนิดข้อมูลที่สําคัญในตัวจะตอบสนองความต้องการของคุณมีเพียงการปรับแต่งไม่กี่คุณสามารถ[ปรับแต่งในตัวชนิดข้อมูลที่สําคัญ](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="aa1e1-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="aa1e1-115">ตัวอย่างเช่น คุณสามารถเพิ่มหรือนําคําหลักออก หรือเพิ่มหรือลบหลักฐานสนับสนุน เช่น วันที่หรือที่อยู่ออกได้</span><span class="sxs-lookup"><span data-stu-id="aa1e1-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="aa1e1-116">**สร้างชนิดข้อมูลที่ละเอียดอ่อนแบบกําหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="aa1e1-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="aa1e1-117">แต่ถ้าคุณต้องการระบุและป้องกันข้อมูลที่สําคัญชนิดอื่น &ทั้งหมด[create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="aa1e1-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="aa1e1-118">**สร้างชนิดข้อมูลที่สําคัญแบบกําหนดเองในการรักษาความปลอดภัย&ศูนย์ควบคุมการปฏิบัติตามกฎระเบียบ PowerShell**</span><span class="sxs-lookup"><span data-stu-id="aa1e1-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="aa1e1-119">สุดท้ายถ้า UI ไม่ได้ให้ตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถสร้าง[ชนิดข้อมูลที่สําคัญที่กําหนดเองในการรักษาความปลอดภัย&ศูนย์การปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="aa1e1-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="aa1e1-120">โดยเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทั้งหมดที่พร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="aa1e1-120">By starting with an XML file, you can use every option available.</span></span>
