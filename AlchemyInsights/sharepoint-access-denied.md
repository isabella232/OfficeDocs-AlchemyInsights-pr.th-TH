---
title: แก้ไขข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691702"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f3bbe-102">แก้ไขข้อความปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="f3bbe-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f3bbe-103">ถ้าคุณได้รับข้อความแสดงข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไซต์ Sharepoint Online โปรดดูที่บทความด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="f3bbe-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="f3bbe-104">**เพิ่มและสิทธิ์การใช้งานผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="f3bbe-104">**Add and License the user**</span></span>

<span data-ttu-id="f3bbe-105">ตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="f3bbe-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="f3bbe-106">**กำหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="f3bbe-106">**Assign Permissions**</span></span>

<span data-ttu-id="f3bbe-107">ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึงโปรดตรวจสอบให้แน่ใจว่ามีการ[กำหนดระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="f3bbe-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="f3bbe-108">**พิจารณาการใช้ฟีเจอร์การร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="f3bbe-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="f3bbe-109">ฟีเจอร์การ [ร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ช่วยให้ผู้อื่นสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับสิทธิ์ในการดู</span><span class="sxs-lookup"><span data-stu-id="f3bbe-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="f3bbe-110">**อนุญาตสคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาในการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="f3bbe-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="f3bbe-111">มีบางสถานการณ์ที่ฟีเจอร์ "อนุญาตให้ใช้สคริปต์แบบกำหนดเอง" อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="f3bbe-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="f3bbe-112">สำหรับรายการของฟีเจอร์ที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานฟีเจอร์นี้</span><span class="sxs-lookup"><span data-stu-id="f3bbe-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="f3bbe-113">โปรดเยี่ยมชม [อนุญาตหรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="f3bbe-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="f3bbe-114">หมายเหตุ: ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="f3bbe-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="f3bbe-115">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="f3bbe-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

