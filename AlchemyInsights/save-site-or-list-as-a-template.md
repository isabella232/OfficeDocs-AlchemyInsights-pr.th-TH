---
title: บันทึกไซต์หรือรายการเป็นแม่แบบ
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752051"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="be4ee-102">บันทึกไซต์หรือรายการเป็นแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="be4ee-102">Save site or list as a template</span></span>

<span data-ttu-id="be4ee-103">แม่แบบไซต์ SharePoint เป็นคำนิยามที่สร้างไว้ล่วงหน้าซึ่งออกแบบมาโดยรอบความต้องการทางธุรกิจที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="be4ee-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="be4ee-104">สำหรับข้อมูลเพิ่มเติมให้ดู[การใช้แม่แบบเพื่อสร้างไซต์ SharePoint ชนิดต่างๆ](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)</span><span class="sxs-lookup"><span data-stu-id="be4ee-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="be4ee-105">ต่อไปนี้เป็นปัญหา/วิธีแก้ไขทั่วไปบางอย่างเกี่ยวกับการบันทึกไซต์หรือรายการเป็นแม่แบบใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="be4ee-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="be4ee-106">**บันทึกปุ่มแม่แบบไซต์/รายการไม่พร้อมใช้งานหรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="be4ee-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="be4ee-107">ผู้ดูแลระบบจะต้องอนุญาตสคริปต์ที่กำหนดเองเพื่อเปิดใช้งานคุณลักษณะแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="be4ee-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="be4ee-108">สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณาที่[สามารถดูอนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="be4ee-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="be4ee-109">คำสั่งบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานการประกาศของเซิร์ฟเวอร์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="be4ee-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="be4ee-110">**ไม่สามารถสร้างแม่แบบไซต์หรือทำงานไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="be4ee-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="be4ee-111">แม่แบบอาจจะหายไป[คุณลักษณะ](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="be4ee-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="be4ee-112">ถ้าคุณลักษณะนี้ไม่พร้อมใช้งานสำหรับการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="be4ee-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="be4ee-113">ตรวจสอบเพื่อดูว่ารายการหรือไลบรารีใดๆเกิน[ขีดจำกัดมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)จำกัดของรายการ๕๐๐๐เช่นนี้สามารถบล็อกการสร้างแม่แบบไซต์</span><span class="sxs-lookup"><span data-stu-id="be4ee-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="be4ee-114">ไซต์นี้อาจจะใช้ทรัพยากรมากเกินไปและแม่แบบไซต์จึงเกินขีดจำกัด๕๐เมกะไบต์ (MB)</span><span class="sxs-lookup"><span data-stu-id="be4ee-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="be4ee-115">มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="be4ee-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="be4ee-116">สำหรับข้อมูลเพิ่มเติมให้ดู[รายการที่สร้างขึ้นโดยแม่แบบไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="be4ee-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="be4ee-117">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาและโซลูชันทั่วไปโปรดอ้างอิง[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="be4ee-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

