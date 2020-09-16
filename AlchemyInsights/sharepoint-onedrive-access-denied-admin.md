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
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767682"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="90b84-102">การแก้ไขปัญหาการเข้าถึงปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="90b84-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="90b84-103">ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไปยังศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="90b84-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="90b84-104">ถ้าผู้ใช้มีสิทธิ์การใช้งานคุณควรตรวจสอบให้แน่ใจว่าผู้ใช้ได้รับ [มอบหมายบทบาทผู้ดูแลระบบ](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ที่สามารถเข้าถึงศูนย์การจัดการได้</span><span class="sxs-lookup"><span data-stu-id="90b84-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="90b84-105">ปัญหานี้อาจเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลักเดียวกัน (UPN)</span><span class="sxs-lookup"><span data-stu-id="90b84-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="90b84-106">บัญชีผู้ใช้ใหม่ถูกสร้างโดยใช้ค่า PUID (ID ที่ไม่ซ้ำกันของ Passport) ที่แตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="90b84-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="90b84-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="90b84-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="90b84-108">สถานการณ์สมมติที่สองจะเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีกับหน่วยองค์กร Active Directory (OU)</span><span class="sxs-lookup"><span data-stu-id="90b84-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="90b84-109">ถ้าผู้ใช้ได้ลงชื่อเข้าใช้ SharePoint เรียบร้อยแล้วและจะถูกย้ายไปยัง OU และ resynced ที่แตกต่างกันกับ SharePoint พวกเขาอาจประสบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="90b84-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="90b84-110">เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN ต้นฉบับที่มีขั้นตอนในบทความให้[คืนค่าผู้ใช้ใน Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="90b84-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="90b84-111">หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงก่อนหน้านี้อาจมีปัญหาในการบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="90b84-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="90b84-112">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="90b84-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


