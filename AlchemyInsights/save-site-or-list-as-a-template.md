---
title: บันทึกไซต์หรือรายการเป็นเทมเพลต
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727550"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="66a86-102">บันทึกไซต์หรือรายการเป็นเทมเพลต</span><span class="sxs-lookup"><span data-stu-id="66a86-102">Save site or list as a template</span></span>

<span data-ttu-id="66a86-103">เทมเพลตของไซต์ SharePoint คือข้อกำหนดสร้างไว้ล่วงที่ได้รับการออกแบบรอบๆความต้องการทางธุรกิจที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="66a86-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="66a86-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การใช้เทมเพลตเพื่อสร้างไซต์ SharePoint ชนิดต่างๆ](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)</span><span class="sxs-lookup"><span data-stu-id="66a86-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="66a86-105">ต่อไปนี้เป็นปัญหาทั่วไป/วิธีแก้ไขปัญหาทั่วไปเกี่ยวกับการบันทึกไซต์หรือรายการเป็นเทมเพลตใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="66a86-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="66a86-106">**ปุ่มบันทึกเทมเพลตไซต์/รายการจะไม่พร้อมใช้งานหรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="66a86-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="66a86-107">ผู้ดูแลระบบจะต้องเปิดใช้งานสคริปต์แบบกำหนดเองเพื่อเปิดใช้งานฟีเจอร์เทมเพลต</span><span class="sxs-lookup"><span data-stu-id="66a86-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="66a86-108">สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณาในการ[อนุญาตหรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="66a86-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="66a86-109">คำสั่งบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานของการประกาศของ SharePoint Server</span><span class="sxs-lookup"><span data-stu-id="66a86-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="66a86-110">**ไม่สามารถสร้างเทมเพลตของไซต์หรือทำงานได้อย่างถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="66a86-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="66a86-111">เทมเพลตนี้อาจไม่มี [ฟีเจอร์](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) และไม่สามารถเปิดใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="66a86-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="66a86-112">ถ้าฟีเจอร์ไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้เทมเพลตของไซต์เพื่อสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="66a86-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="66a86-113">ตรวจสอบดูว่ารายการหรือไลบรารีใดที่เกินขีด [จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ของรายการ๕๐๐๐เนื่องจากการทำเช่นนี้สามารถบล็อกการสร้างเทมเพลตของไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="66a86-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="66a86-114">ไซต์อาจใช้แหล่งข้อมูลมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐เมกะไบต์ (MB)</span><span class="sxs-lookup"><span data-stu-id="66a86-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="66a86-115">มีปัญหาเกิดขึ้นในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="66a86-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="66a86-116">สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการที่สร้างขึ้นโดยใช้เทมเพลตไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="66a86-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="66a86-117">สำหรับข้อมูลรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาทั่วไปและการแก้ไขปัญหาโปรดอ้างอิง[สร้างและใช้เทมเพลตของไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="66a86-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

