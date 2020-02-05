---
title: สร้างไซต์ใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770442"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="a457c-102">การสร้างไซต์ SharePoint โดยใช้แม่แบบ</span><span class="sxs-lookup"><span data-stu-id="a457c-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="a457c-103">ความสามารถในการบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนด้วยการสื่อสารที่ทันสมัยหรือเว็บไซต์ทีม</span><span class="sxs-lookup"><span data-stu-id="a457c-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="a457c-104">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการใช้แม่แบบดู[บันทึกดาวน์โหลดและอัปโหลดไซต์ SharePoint เป็นแม่แบบ](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)</span><span class="sxs-lookup"><span data-stu-id="a457c-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="a457c-105">ต่อไปนี้เป็นปัญหาทั่วไปบางส่วน/การแก้ไขปัญหาเกี่ยวกับการบันทึกไซต์หรือรายการเป็นแม่แบบใน Sharepoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="a457c-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="a457c-106">**บันทึกปุ่มแม่แบบของไซต์/รายการไม่พร้อมใช้งานหรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="a457c-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="a457c-107">ผู้ดูแลระบบจะต้องอนุญาตให้สคริปต์ที่กำหนดเองเพื่อเปิดใช้งานคุณลักษณะแม่แบบ</span><span class="sxs-lookup"><span data-stu-id="a457c-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="a457c-108">สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณา</span><span class="sxs-lookup"><span data-stu-id="a457c-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="a457c-109">อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="a457c-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="a457c-110">คำสั่งบันทึกไซต์เป็นแม่แบบไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานการเผยแพร่เซิร์ฟเวอร์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="a457c-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="a457c-111">**ไม่สามารถสร้างแม่แบบไซต์หรือทำงานไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="a457c-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="a457c-112">แม่แบบอาจขาด[คุณลักษณะ](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)และจะไม่เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="a457c-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="a457c-113">ถ้าคุณลักษณะไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="a457c-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="a457c-114">ตรวจสอบดูว่ามีรายการหรือไลบรารีเกินขีด[จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)ของ๕๐๐๐รายการในขณะนี้สามารถบล็อกการสร้างแม่แบบไซต์</span><span class="sxs-lookup"><span data-stu-id="a457c-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="a457c-115">ไซต์อาจใช้ทรัพยากรมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐ MB</span><span class="sxs-lookup"><span data-stu-id="a457c-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="a457c-116">มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="a457c-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="a457c-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการสร้างแม่แบบไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="a457c-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="a457c-118">สำหรับข้อมูลรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาและวิธีการแก้ไขทั่วไปโปรดตรวจสอบการ[สร้างและใช้แม่แบบไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="a457c-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



