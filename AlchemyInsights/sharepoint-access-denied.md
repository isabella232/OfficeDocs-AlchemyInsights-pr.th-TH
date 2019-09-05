---
title: การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 915476f92f150288666268f1647f3cae7e9001a4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751799"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="eb3da-102">การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="eb3da-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="eb3da-103">ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไซต์ Sharepoint แบบออนไลน์โปรดดูที่บทความด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="eb3da-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="eb3da-104">**เพิ่มและอนุญาตให้ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="eb3da-104">**Add and License the user**</span></span>

<span data-ttu-id="eb3da-105">ตรวจสอบให้แน่ใจว่าคุณได้[มอบหมายใบอนุญาตให้กับผู้ใช้ใน Office ๓๖๕สำหรับธุรกิจ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="eb3da-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="eb3da-106">**กำหนดสิทธิ์**</span><span class="sxs-lookup"><span data-stu-id="eb3da-106">**Assign Permissions**</span></span>

<span data-ttu-id="eb3da-107">ถ้าผู้ใช้ได้รับการกำหนดใบอนุญาต Sharepoint และยังคงได้รับข้อความการเข้าถึงถูกปฏิเสธโปรดตรวจสอบให้แน่ใจว่ามีการ[กำหนดระดับสิทธิ์ที่เหมาะสม](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="eb3da-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="eb3da-108">**พิจารณาการใช้คุณลักษณะการร้องขอการเข้าถึง**</span><span class="sxs-lookup"><span data-stu-id="eb3da-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="eb3da-109">คุณลักษณะการ[ร้องขอการเข้าถึง](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)ช่วยให้ผู้คนสามารถร้องขอการเข้าถึงเนื้อหาที่พวกเขาไม่ได้รับอนุญาตให้ดูได้ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="eb3da-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="eb3da-110">**อนุญาตสคริปต์ที่กำหนดเองอาจทำให้เกิดปัญหาการเข้าถึงถูกปฏิเสธ**</span><span class="sxs-lookup"><span data-stu-id="eb3da-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="eb3da-111">มีบางสถานการณ์ที่คุณลักษณะ "อนุญาตให้ใช้สคริปต์ที่กำหนดเอง" อาจนำเสนอการเข้าถึงถูกปฏิเสธ</span><span class="sxs-lookup"><span data-stu-id="eb3da-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="eb3da-112">สำหรับรายการของคุณลักษณะที่ได้รับผลกระทบข้อควรพิจารณาด้านความปลอดภัยและความสามารถในการปิดใช้งานคุณลักษณะนี้</span><span class="sxs-lookup"><span data-stu-id="eb3da-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="eb3da-113">กรุณาเยี่ยมชม,[อนุญาตหรือป้องกันสคริปต์ที่กำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="eb3da-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="eb3da-114">หมายเหตุ: ถ้าเว็บไซต์ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร</span><span class="sxs-lookup"><span data-stu-id="eb3da-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="eb3da-115">[ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="eb3da-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

