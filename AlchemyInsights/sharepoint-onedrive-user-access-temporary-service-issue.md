---
title: ปัญหาด้านประสิทธิภาพการทำงาน-SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771263"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a2e3a-102">SharePoint หรือ OneDrive ช้าไม่สามารถเข้าถึงหรือไม่พร้อมใช้งานสำหรับผู้ใช้หลายคน</span><span class="sxs-lookup"><span data-stu-id="a2e3a-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="a2e3a-103">ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="a2e3a-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a2e3a-104">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a2e3a-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="a2e3a-105">**เพิ่มและสิทธิ์การใช้งานผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="a2e3a-105">**Add and license the user**</span></span>

<span data-ttu-id="a2e3a-106">ตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="a2e3a-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="a2e3a-107">**กำหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="a2e3a-107">**Assign Permissions**</span></span>

<span data-ttu-id="a2e3a-108">ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึงโปรดตรวจสอบให้แน่ใจว่ามีการกำหนด[ระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="a2e3a-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="a2e3a-109">**พิจารณาการใช้ฟีเจอร์การร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="a2e3a-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="a2e3a-110">[ฟีเจอร์การร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)ช่วยให้ผู้อื่นสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับสิทธิ์ในการดู</span><span class="sxs-lookup"><span data-stu-id="a2e3a-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="a2e3a-111">**อนุญาตสคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาในการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="a2e3a-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="a2e3a-112">มีบางสถานการณ์ที่การอนุญาตให้ใช้ฟีเจอร์ *สคริปต์แบบกำหนดเอง* อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="a2e3a-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="a2e3a-113">สำหรับรายการของฟีเจอร์ที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานฟีเจอร์นี้</span><span class="sxs-lookup"><span data-stu-id="a2e3a-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a2e3a-114">โปรดเยี่ยมชม[อนุญาตหรือป้องกันสคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="a2e3a-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

