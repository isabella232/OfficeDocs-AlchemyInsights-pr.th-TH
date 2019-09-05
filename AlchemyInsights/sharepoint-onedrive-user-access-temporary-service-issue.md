---
title: ปัญหาประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750575"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="7cbe8-102">SharePoint หรือ OneDrive ช้า, ไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="7cbe8-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="7cbe8-103">ถ้าเว็บไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร</span><span class="sxs-lookup"><span data-stu-id="7cbe8-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="7cbe8-104">[ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="7cbe8-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="7cbe8-105">**เพิ่มและอนุญาตให้ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="7cbe8-105">**Add and license the user**</span></span>

<span data-ttu-id="7cbe8-106">ตรวจสอบให้แน่ใจว่าคุณได้[มอบหมายใบอนุญาตให้กับผู้ใช้ใน Office ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="7cbe8-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="7cbe8-107">**กำหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="7cbe8-107">**Assign Permissions**</span></span>

<span data-ttu-id="7cbe8-108">ถ้าผู้ใช้ได้รับการกำหนดใบอนุญาต Sharepoint และยังคงได้รับข้อความการเข้าถึงถูกปฏิเสธโปรดตรวจสอบให้แน่ใจว่ามีการกำหนด[ระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="7cbe8-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="7cbe8-109">**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="7cbe8-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="7cbe8-110">[คุณลักษณะการร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)ช่วยให้ผู้คนสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขาไม่ได้รับอนุญาตให้ดูได้ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="7cbe8-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="7cbe8-111">**อนุญาตสคริปต์ที่กำหนดเองอาจทำให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="7cbe8-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="7cbe8-112">มีบางสถานการณ์ที่การอนุญาตให้ใช้คุณลักษณะของ*สคริปต์ที่กำหนดเอง*อาจนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="7cbe8-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="7cbe8-113">สำหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะนี้</span><span class="sxs-lookup"><span data-stu-id="7cbe8-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="7cbe8-114">โปรดเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="7cbe8-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

