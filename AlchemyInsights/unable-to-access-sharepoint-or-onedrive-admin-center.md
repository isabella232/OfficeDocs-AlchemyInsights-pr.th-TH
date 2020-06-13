---
title: ไม่สามารถเข้าถึง SharePoint หรือศูนย์การจัดการ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716474"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="9ec82-102">ไม่สามารถเข้าถึง SharePoint หรือศูนย์การจัดการ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9ec82-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="9ec82-103">ถ้าไซต์ศูนย์การดูแล SharePoint หรือ OneDrive ของคุณไม่สามารถเข้าถึงหรือไม่พร้อมใช้งาน อาจมีปัญหาการบริการชั่วคราวที่ผู้ใช้พบความล่าช้าเป็นระยะ ๆ หรือข้อผิดพลาดในการนําทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหาของ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9ec82-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="9ec82-104">ตรวจสอบ[แดชบอร์ดสถานภาพบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="9ec82-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="9ec82-105">ผู้ดูแลระบบส่วนกลางและ SharePoint ต้องได้รับมอบหมายสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="9ec82-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="9ec82-106">บัญชีที่สร้างขึ้นใหม่เพิ่งได้รับมอบหมายด้วยบทบาทสิทธิ์การใช้งาน SharePoint หรือผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="9ec82-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="9ec82-107">โปรดให้อย่างน้อย 24 ชั่วโมงสําหรับการซิงค์เพื่อให้เสร็จสมบูรณ์ในระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="9ec82-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="9ec82-108">เราเข้าใจว่า 24 ชั่วโมงอาจดูเหมือนเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="9ec82-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="9ec82-109">ในหลายกรณีเรากําลังทํางานอยู่แล้วในการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="9ec82-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="9ec82-110">ผู้ใช้การจัดการข้อมูลเฉพาะตัวที่มีสิทธิ์ ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) อาจได้รับการปฏิเสธการเข้าถึงถ้าหน้าต่างเวลาการเข้าถึงที่ได้รับอนุญาตมีขนาดเล็กมาก ให้ดูที่[การเข้าถึงถูกปฏิเสธไปยังบัญชี PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="9ec82-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>