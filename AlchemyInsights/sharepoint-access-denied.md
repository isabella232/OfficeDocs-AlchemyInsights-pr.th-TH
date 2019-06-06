---
title: การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735756"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="373e1-102">การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="373e1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="373e1-103">หากคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อคุณพยายามเรียกดูไซต์ Sharepoint แบบออนไลน์ โปรดดูด้านล่างของบทความ</span><span class="sxs-lookup"><span data-stu-id="373e1-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="373e1-104">เพิ่ม และสิทธิ์การใช้งานของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="373e1-104">Add and License the user</span></span>

<span data-ttu-id="373e1-105">ให้แน่ใจว่าคุณ[กำหนดสิทธิ์การใช้งานสำหรับผู้ใช้ใน Office 365 สำหรับธุรกิจ](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="373e1-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="373e1-106">กำหนดการอนุญาต</span><span class="sxs-lookup"><span data-stu-id="373e1-106">Assign Permissions</span></span>

<span data-ttu-id="373e1-107">ถ้าผู้ใช้มีการกำหนดสิทธิ์การใช้งาน Sharepoint และยังคงได้รับการเข้าถึงถูกปฏิเสธข้อความ โปรดตรวจสอบว่ามีการ[กำหนดระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="373e1-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="373e1-108">พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="373e1-108">Consider using the access request feature</span></span>

<span data-ttu-id="373e1-109">[ร้องขอการเข้าถึง](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)คุณลักษณะช่วยให้บุคคลที่จะร้องขอการเข้าถึงเนื้อหาที่พวกเขายังไม่ได้รับอนุญาตให้ดู</span><span class="sxs-lookup"><span data-stu-id="373e1-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="373e1-110">อนุญาตให้ใช้สคริปต์แบบกำหนดเองอาจทำให้เกิดปัญหาปฏิเสธการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="373e1-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="373e1-111">มีบางสถานการณ์ที่คุณลักษณะ "อนุญาตสคริปต์แบบกำหนดเอง" อาจจะนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="373e1-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="373e1-112">สำหรับรายการของลักษณะการทำงานที่ได้รับผลกระทบ ข้อควรพิจารณาด้านความปลอดภัย และความสามารถในการปิดใช้งานลักษณะการทำงาน</span><span class="sxs-lookup"><span data-stu-id="373e1-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="373e1-113">โปรดเยี่ยมชม[อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="373e1-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="373e1-114">หมายเหตุ: ถ้าไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้ มีการเข้าถึงไซต์ SharePoint หรือการ OneDrive อาจมีปัญหากับบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="373e1-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="373e1-115">[ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="373e1-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

