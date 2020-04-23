---
title: การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: a1541aa401efbc03e8a6104ba435c7fdf20a977a
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742162"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="3a683-102">การแก้ไขปัญหาข้อความปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="3a683-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="3a683-103">หากคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไซต์ Sharepoint Online โปรดดูบทความด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="3a683-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="3a683-104">**เพิ่มและสิทธิ์การใช้งานผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="3a683-104">**Add and License the user**</span></span>

<span data-ttu-id="3a683-105">ตรวจสอบให้แน่ใจว่าคุณ[กําหนดสิทธิ์การใช้งานให้กับผู้ใช้ใน Microsoft 365 สําหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="3a683-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="3a683-106">**กําหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="3a683-106">**Assign Permissions**</span></span>

<span data-ttu-id="3a683-107">ถ้าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งาน Sharepoint และยังคงได้รับข้อความปฏิเสธการเข้าถึง โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ[สิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="3a683-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="3a683-108">**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="3a683-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="3a683-109">คุณลักษณะ[การร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)อนุญาตให้บุคคลอื่นร้องขอการเข้าถึงเนื้อหาที่ไม่ได้รับอนุญาติให้ดูในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="3a683-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="3a683-110">**อนุญาตสคริปต์แบบกําหนดเองอาจทําให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="3a683-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="3a683-111">มีบางสถานการณ์ที่คุณลักษณะ "อนุญาตสคริปต์แบบกําหนดเอง" อาจแสดงการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="3a683-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="3a683-112">สําหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะ</span><span class="sxs-lookup"><span data-stu-id="3a683-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="3a683-113">กรุณาเยี่ยมชม ,[อนุญาตหรือป้องกันสคริปต์ที่กําหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="3a683-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="3a683-114">หมายเหตุ: ถ้าไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสําหรับผู้ใช้หลายคนที่เคยมีการเข้าถึง อาจมีปัญหาการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="3a683-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="3a683-115">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="3a683-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

