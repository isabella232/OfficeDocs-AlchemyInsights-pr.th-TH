---
title: ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749497"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="2f620-102">ไม่สามารถเข้าถึงศูนย์การจัดการ SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f620-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="2f620-103">ถ้าไซต์ SharePoint หรือศูนย์การจัดการ OneDrive ของคุณไม่สามารถเข้าถึงได้หรือไม่พร้อมใช้งานอาจมีปัญหาด้านบริการชั่วคราวที่ผู้ใช้พบความล่าช้าหรือข้อผิดพลาดในการนำทางเมื่อเข้าถึงไซต์ SharePoint หรือเนื้อหา OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f620-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="2f620-104">ตรวจสอบ [แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) เพื่อดูว่าองค์กรของคุณได้รับผลกระทบหรือไม่</span><span class="sxs-lookup"><span data-stu-id="2f620-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="2f620-105">ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="2f620-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="2f620-106">บัญชีผู้ใช้ที่สร้างขึ้นใหม่เพิ่งมอบหมายให้กับสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "access denied" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="2f620-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="2f620-107">โปรดให้การซิงค์อย่างน้อย24ชั่วโมงเพื่อให้เสร็จสมบูรณ์ในระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="2f620-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="2f620-108">เราเข้าใจว่า24ชั่วโมงอาจดูเหมือนเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="2f620-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="2f620-109">ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="2f620-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="2f620-110">ผู้ใช้ที่มีสิทธิ์ในการจัดการข้อมูลประจำตัว ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) อาจได้รับการเข้าถึงถูกปฏิเสธถ้าหน้าต่างเวลาการเข้าถึงที่อนุญาตมีขนาดเล็กมากให้ดู[การเข้าถึงถูกปฏิเสธไปยังบัญชีผู้ใช้ PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="2f620-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>