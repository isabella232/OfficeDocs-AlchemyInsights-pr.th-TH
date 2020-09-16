---
title: การสร้างไซต์ใน SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732262"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="5b1b3-102">การสร้างไซต์ SharePoint โดยใช้เทมเพลต</span><span class="sxs-lookup"><span data-stu-id="5b1b3-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="5b1b3-103">ความสามารถในการบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนด้วยการติดต่อสื่อสารหรือไซต์ทีมที่ทันสมัย</span><span class="sxs-lookup"><span data-stu-id="5b1b3-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="5b1b3-104">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการใช้เทมเพลตให้ดูที่[บันทึกดาวน์โหลดและอัปโหลดไซต์ SharePoint เป็นเทมเพลต](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)</span><span class="sxs-lookup"><span data-stu-id="5b1b3-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="5b1b3-105">ต่อไปนี้เป็นปัญหาทั่วไป/วิธีแก้ไขปัญหาทั่วไปเกี่ยวกับการบันทึกไซต์หรือรายการเป็นเทมเพลตใน Sharepoint Online</span><span class="sxs-lookup"><span data-stu-id="5b1b3-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="5b1b3-106">**ปุ่มบันทึกเทมเพลตไซต์/รายการไม่พร้อมใช้งานหรือหายไป**</span><span class="sxs-lookup"><span data-stu-id="5b1b3-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="5b1b3-107">ผู้ดูแลระบบจะต้องเปิดใช้งานสคริปต์แบบกำหนดเองเพื่อเปิดใช้งานฟีเจอร์เทมเพลต</span><span class="sxs-lookup"><span data-stu-id="5b1b3-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5b1b3-108">สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณา</span><span class="sxs-lookup"><span data-stu-id="5b1b3-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="5b1b3-109">อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="5b1b3-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="5b1b3-110">คำสั่งบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานของการประกาศของ SharePoint Server</span><span class="sxs-lookup"><span data-stu-id="5b1b3-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="5b1b3-111">**ไม่สามารถสร้างเทมเพลตของไซต์หรือทำงานได้อย่างถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="5b1b3-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="5b1b3-112">เทมเพลตนี้อาจไม่มี [ฟีเจอร์](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) และไม่สามารถเปิดใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="5b1b3-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="5b1b3-113">ถ้าฟีเจอร์ไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้เทมเพลตของไซต์เพื่อสร้างไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="5b1b3-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="5b1b3-114">ตรวจสอบดูว่ารายการหรือไลบรารีใดที่เกินขีด [จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ของรายการ๕๐๐๐เนื่องจากการทำเช่นนี้สามารถบล็อกการสร้างเทมเพลตของไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="5b1b3-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="5b1b3-115">ไซต์อาจใช้แหล่งข้อมูลมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐ MB</span><span class="sxs-lookup"><span data-stu-id="5b1b3-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="5b1b3-116">มีปัญหาเกิดขึ้นในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="5b1b3-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5b1b3-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการที่สร้างขึ้นโดยใช้เทมเพลตไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="5b1b3-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="5b1b3-118">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาทั่วไปและการแก้ไขปัญหาโปรดตรวจสอบการ[สร้างและใช้เทมเพลตของไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="5b1b3-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



