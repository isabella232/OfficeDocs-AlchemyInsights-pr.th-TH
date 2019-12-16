---
title: DLP อาจต้องการชนิดที่กำหนดเอง
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052920"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="de55f-102">DLP อาจต้องการชนิดที่กำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="de55f-102">DLP might need a custom type</span></span>

<span data-ttu-id="de55f-103">ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและปกป้องข้อมูลที่สำคัญในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="de55f-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="de55f-104">ในบางสถานการณ์คุณอาจต้องสร้างชนิดข้อมูลที่ละเอียด**อ่อนของคุณเองเพื่อ**ปกป้องข้อมูลขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="de55f-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="de55f-105">ตัวอย่างเช่นองค์กรของคุณอาจจำเป็นต้องระบุและปกป้องรหัสพนักงานหรือข้อมูลอื่นๆในรูปแบบบางอย่างที่เฉพาะเจาะจงกับองค์กรของคุณ หากเป็นเช่นนั้นให้ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="de55f-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="de55f-106">**การกำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**</span><span class="sxs-lookup"><span data-stu-id="de55f-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="de55f-107">ถ้าชนิดข้อมูลที่ละเอียดอ่อนในตัวจะตอบสนองความต้องการของคุณด้วยการปรับแต่งเพียงไม่กี่คุณสามารถ[กำหนดชนิดข้อมูลที่มีความละเอียดอ่อนในตัว](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)ได้</span><span class="sxs-lookup"><span data-stu-id="de55f-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="de55f-108">ตัวอย่างเช่นคุณสามารถเพิ่มหรือเอาคำสำคัญออกหรือเพิ่มหรือลบหลักฐานที่สนับสนุนเช่นวันที่หรือที่อยู่</span><span class="sxs-lookup"><span data-stu-id="de55f-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="de55f-109">**การสร้างชนิดข้อมูลที่เป็นความลับที่กำหนดเอง**</span><span class="sxs-lookup"><span data-stu-id="de55f-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="de55f-110">แต่ถ้าคุณต้องการระบุและปกป้องข้อมูลที่ละเอียดอ่อนชนิดอื่นทั้งหมดคุณสามารถ[สร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)ใน UI ของศูนย์การปฏิบัติตามกฎระเบียบ &</span><span class="sxs-lookup"><span data-stu-id="de55f-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="de55f-111">**สร้างชนิดข้อมูลที่ละเอียดอ่อนที่กำหนดเองใน PowerShell ศูนย์ปฏิบัติตามกฎระเบียบ & ความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="de55f-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="de55f-112">ในที่สุดถ้า UI ไม่มีตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถ[สร้างชนิดข้อมูลที่เป็นความลับที่กำหนดเองได้ในการปฏิบัติตามข้อบังคับ & PowerShell ศูนย์กลาง](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="de55f-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="de55f-113">โดยการเริ่มต้นด้วยแฟ้ม XML คุณสามารถใช้ตัวเลือกทุกอย่างได้</span><span class="sxs-lookup"><span data-stu-id="de55f-113">By starting with an XML file, you can use every option available.</span></span>
