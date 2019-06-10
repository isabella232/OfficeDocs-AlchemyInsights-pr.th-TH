---
title: บันทึกไซต์หรือรายการเป็นแม่แบบ
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770546"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="2f56c-102">บันทึกไซต์หรือรายการเป็นแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="2f56c-102">Save site or list as a template</span></span>

<span data-ttu-id="2f56c-103">แม่แบบไซต์ SharePoint จะปรากฏคำนิยามที่ออกแบบมาให้อยู่รอบ ๆ ความต้องการเฉพาะทางด้านธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="2f56c-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="2f56c-104">ดูข้อมูลเพิ่มเติม[ใช้แม่แบบเพื่อสร้างชนิดของไซต์ SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)</span><span class="sxs-lookup"><span data-stu-id="2f56c-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="2f56c-105">ต่อไปนี้เป็นปัญหา/แก้ไขปัญหาทั่วไปบางอย่างเกี่ยวกับการบันทึกเป็นไซต์หรือรายการเป็นแม่แบบใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="2f56c-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="2f56c-106">**บันทึกลงรายการไซต์ แม่แบบปุ่มจะไม่พร้อมใช้งาน หรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="2f56c-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="2f56c-107">ผู้ดูแลจะต้องใช้เมื่อต้องการอนุญาตให้ใช้สคริปต์แบบกำหนดเองเพื่อเปิดใช้งานลักษณะการทำงานของแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="2f56c-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="2f56c-108">สำหรับขั้นตอนโดยละเอียด ตัวอย่าง และข้อควรพิจารณาดู[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="2f56c-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="2f56c-109">ไซต์บันทึกแม่แบบในคำสั่งไม่ได้รับการสนับสนุน และอาจทำให้เกิดปัญหาบนไซต์ที่ใช้ SharePoint Server ประกาศโครงสร้างพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="2f56c-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="2f56c-110">**แม่แบบไซต์ไม่สามารถสร้าง หรือทำงานไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="2f56c-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="2f56c-111">แม่แบบนี้อาจไม่มี[ลักษณะการทำงาน](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2f56c-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="2f56c-112">ถ้าคุณลักษณะนี้ไม่พร้อมใช้งานเพื่อเรียกใช้งานในไซต์คอลเลกชันปัจจุบัน คุณไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="2f56c-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="2f56c-113">ตรวจสอบถ้ารายการหรือไลบรารีใด ๆ เกิน[ขีดจำกัดมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)ของสินค้า 5000 ขณะนี้สามารถบล็อคการสร้างแม่แบบไซต์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="2f56c-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="2f56c-114">ไซต์อาจจะกำลังใช้ทรัพยากรมากเกินไป และดังนั้น แม่แบบไซต์เกินขีดจำกัด 50 เมกะไบต์ (MB)</span><span class="sxs-lookup"><span data-stu-id="2f56c-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="2f56c-115">มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์ค้นหา</span><span class="sxs-lookup"><span data-stu-id="2f56c-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="2f56c-116">สำหรับข้อมูลเพิ่มเติม ดู[สร้างแม่แบบรายการไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)</span><span class="sxs-lookup"><span data-stu-id="2f56c-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="2f56c-117">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาทั่วไปและการแก้ไขปัญหาโปรดอ้างอิง การ[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="2f56c-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

