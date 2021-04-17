---
title: ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824454"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="f0e66-102">ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive ได้</span><span class="sxs-lookup"><span data-stu-id="f0e66-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="f0e66-103">ถ้าไซต์ศูนย์การจัดการ SharePoint หรือ OneDrive ของคุณไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งาน อาจมีปัญหาชั่วคราวที่ผู้ใช้พบความล่าช้าหรือการนําทางที่ผิดพลาดเป็นระยะๆ เมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive</span><span class="sxs-lookup"><span data-stu-id="f0e66-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="f0e66-104">ตรวจสอบ [แดชบอร์ดสถานภาพ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) บริการเพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f0e66-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="f0e66-105">ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint ต้องได้รับการมอบหมายสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="f0e66-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="f0e66-106">บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="f0e66-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="f0e66-107">โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="f0e66-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="f0e66-108">เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="f0e66-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="f0e66-109">ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="f0e66-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="f0e66-110">ผู้ใช้การจัดการข้อมูลเฉพาะตัวที่ได้รับ[สิทธิ์ (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)อาจถูกปฏิเสธการเข้าถึงถ้าหน้าต่างเวลาการเข้าถึงที่อนุญาตมีขนาดเล็กมาก ให้ดู[การเข้าถึงถูกปฏิเสธบัญชี PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="f0e66-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>