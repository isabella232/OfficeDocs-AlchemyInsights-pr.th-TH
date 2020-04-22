---
title: ปัญหาประสิทธิภาพการทํางาน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692712"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="f314d-102">SharePoint หรือ OneDrive ช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานสําหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="f314d-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="f314d-103">ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="f314d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="f314d-104">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="f314d-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="f314d-105">**เพิ่มและอนุญาตผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="f314d-105">**Add and license the user**</span></span>

<span data-ttu-id="f314d-106">ตรวจสอบให้แน่ใจว่าคุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft 365 สําหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="f314d-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="f314d-107">**กําหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="f314d-107">**Assign Permissions**</span></span>

<span data-ttu-id="f314d-108">ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึง โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[สิทธิ์ที่เหมาะสมที่กําหนด](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="f314d-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="f314d-109">**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="f314d-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="f314d-110">[คุณลักษณะการร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้บุคคลอื่นร้องขอการเข้าถึงเนื้อหาที่ไม่ได้รับอนุญาติให้ดูในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="f314d-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="f314d-111">**อนุญาตสคริปต์แบบกําหนดเองอาจทําให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="f314d-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="f314d-112">มีบางสถานการณ์ที่คุณลักษณะ*การอนุญาตให้สคริปต์แบบกําหนดเอง*อาจนําเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="f314d-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="f314d-113">สําหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะ</span><span class="sxs-lookup"><span data-stu-id="f314d-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="f314d-114">กรุณาเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="f314d-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

