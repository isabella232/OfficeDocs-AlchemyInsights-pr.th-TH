---
title: DLP อาจจำเป็นต้องเป็นชนิดกำหนดเอง
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399133"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="b623a-102">DLP อาจจำเป็นต้องเป็นชนิดกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="b623a-102">DLP might need a custom type</span></span>

<span data-ttu-id="b623a-103">นโยบาย (DLP) การป้องกันข้อมูลสูญหาย คุณสามารถระบุ และป้องกันข้อมูลที่สำคัญในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b623a-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="b623a-104">ในบางสถานการณ์ คุณอาจต้องการสร้างชนิดข้อมูลที่เป็นความลับของผู้ใช้**แบบกำหนดเอง**เพื่อปกป้องข้อมูลขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b623a-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="b623a-105">ตัวอย่างเช่น ที่องค์กรของคุณอาจจำเป็นต้องระบุ และป้องกันรหัสพนักงานหรือข้อมูลอื่น ๆ ในบางรูปแบบเฉพาะในชื่อของคุณ ถ้าเป็นเช่นนั้น ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b623a-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="b623a-106">**กำหนดชนิดข้อมูลที่สำคัญอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="b623a-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="b623a-107">ถ้าชนิดข้อมูลที่สำคัญอยู่แล้วภายในจะต้องตรงกับความต้องการของคุณ มีเพียงไม่กี่ tweaks คุณสามารถ[กำหนดชนิดข้อมูลที่สำคัญอยู่แล้วภายใน](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="b623a-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="b623a-108">ตัวอย่างเช่น คุณสามารถเพิ่ม หรือเอาคำสำคัญ หรือเพิ่ม หรือเอาหลักฐานที่สนับสนุนเช่นวันหรือที่อยู่</span><span class="sxs-lookup"><span data-stu-id="b623a-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="b623a-109">**สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ**</span><span class="sxs-lookup"><span data-stu-id="b623a-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="b623a-110">แต่ถ้าคุณจำเป็นต้องระบุ และปกป้องข้อมูลสำคัญชนิดอื่นทั้งหมด คุณสามารถ[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญ](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type)ใน UI ของ & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="b623a-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="b623a-111">**สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญในการรักษาความปลอดภัย & PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ**</span><span class="sxs-lookup"><span data-stu-id="b623a-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="b623a-112">ในตอนท้าย ถ้า UI ไม่ได้จัดเตรียมตัวเลือกทั้งหมดที่คุณจำเป็น คุณสามารถ[สร้างชนิดข้อมูลแบบกำหนดเองที่สำคัญในการรักษาความปลอดภัย & PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="b623a-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="b623a-113">โดยเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทุกตัวพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="b623a-113">By starting with an XML file, you can use every option available.</span></span>

    
