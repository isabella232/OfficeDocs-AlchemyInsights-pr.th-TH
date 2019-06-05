---
title: ปัญหาเกี่ยวกับประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719535"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="149b1-102">SharePoint หรือ OneDrive ช้า ไม่สามารถเข้าถึง หรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="149b1-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="149b1-103">ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้ มีการเข้าถึงไซต์ SharePoint หรือการ OneDrive อาจมีปัญหากับบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="149b1-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="149b1-104">[ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="149b1-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="149b1-105">เพิ่ม และสิทธิ์การใช้งานของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="149b1-105">Add and license the user</span></span>

<span data-ttu-id="149b1-106">ให้แน่ใจว่าคุณ[กำหนดสิทธิ์การใช้งานสำหรับผู้ใช้ใน Office 365 สำหรับธุรกิจ](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="149b1-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="149b1-107">กำหนดการอนุญาต</span><span class="sxs-lookup"><span data-stu-id="149b1-107">Assign Permissions</span></span>

<span data-ttu-id="149b1-108">ถ้าผู้ใช้มีการกำหนดสิทธิ์การใช้งาน Sharepoint และยังคงได้รับการเข้าถึงถูกปฏิเสธข้อความ โปรดให้แน่ใจว่า พวกเขาได้[ระดับของสิทธิ์ที่](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)กำหนดให้</span><span class="sxs-lookup"><span data-stu-id="149b1-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="149b1-109">พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="149b1-109">Consider using the access request feature</span></span>

<span data-ttu-id="149b1-110">การ[เข้าถึงลักษณะการทำงานขอ](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้บุคคลที่จะร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับอนุญาตให้ดู</span><span class="sxs-lookup"><span data-stu-id="149b1-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="149b1-111">อนุญาตให้ใช้สคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="149b1-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="149b1-112">มีบางสถานการณ์ที่คุณลักษณะที่*อนุญาตให้สคริปต์ที่กำหนดเอง*อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="149b1-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="149b1-113">สำหรับรายการของลักษณะการทำงานที่ได้รับผลกระทบ ข้อควรพิจารณาด้านความปลอดภัย และความสามารถในการปิดใช้งานลักษณะการทำงาน</span><span class="sxs-lookup"><span data-stu-id="149b1-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="149b1-114">โปรดเยี่ยมชม[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="149b1-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

