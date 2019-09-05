---
title: สร้างไซต์ใน SharePoint แบบออนไลน์
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755327"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="943d5-102">สร้างไซต์ SharePoint โดยใช้แม่แบบ</span><span class="sxs-lookup"><span data-stu-id="943d5-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="943d5-103">แม่แบบไซต์ SharePoint เป็นคำนิยามที่สร้างไว้ล่วงหน้าซึ่งออกแบบมาโดยรอบความต้องการทางธุรกิจที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="943d5-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="943d5-104">สำหรับข้อมูลเพิ่มเติมให้ดู[การใช้แม่แบบเพื่อสร้างไซต์ SharePoint ชนิดต่างๆ](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)</span><span class="sxs-lookup"><span data-stu-id="943d5-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="943d5-105">ต่อไปนี้เป็นปัญหา/วิธีแก้ไขทั่วไปบางอย่างเกี่ยวกับการบันทึกไซต์หรือรายการเป็นแม่แบบใน Sharepoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="943d5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="943d5-106">**บันทึกปุ่มแม่แบบไซต์/รายการไม่พร้อมใช้งานหรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="943d5-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="943d5-107">ผู้ดูแลระบบจะต้องอนุญาตสคริปต์ที่กำหนดเองเพื่อเปิดใช้งานคุณลักษณะแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="943d5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="943d5-108">สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณาที่เห็น</span><span class="sxs-lookup"><span data-stu-id="943d5-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="943d5-109">อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="943d5-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="943d5-110">คำสั่งบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานการประกาศของเซิร์ฟเวอร์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="943d5-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="943d5-111">**ไม่สามารถสร้างแม่แบบไซต์หรือทำงานไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="943d5-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="943d5-112">แม่แบบอาจจะหายไป[คุณลักษณะ](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="943d5-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="943d5-113">ถ้าคุณลักษณะนี้ไม่พร้อมใช้งานสำหรับการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="943d5-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="943d5-114">ตรวจสอบเพื่อดูว่ารายการหรือไลบรารีใดๆเกิน[ขีดจำกัดมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)จำกัดของรายการ๕๐๐๐เช่นนี้สามารถบล็อกการสร้างแม่แบบไซต์</span><span class="sxs-lookup"><span data-stu-id="943d5-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="943d5-115">ไซต์นี้อาจใช้ทรัพยากรมากเกินไปและแม่แบบไซต์เกินขีดจำกัด๕๐ MB</span><span class="sxs-lookup"><span data-stu-id="943d5-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="943d5-116">มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="943d5-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="943d5-117">สำหรับข้อมูลเพิ่มเติมให้ดู[รายการที่สร้างขึ้นโดยแม่แบบไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="943d5-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="943d5-118">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีแก้ไขทั่วไปโปรดตรวจสอบ[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="943d5-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



