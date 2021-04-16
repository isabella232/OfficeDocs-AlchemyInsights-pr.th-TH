---
title: ผู้ดูแลระบบส่วนกลางและ SharePoint
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
- "9002962"
- "5674"
ms.openlocfilehash: 91abc97be5d616392f8d04b3641af3c9dd8bfd74
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811907"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="45b2e-102">ผู้ดูแลระบบส่วนกลางและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="45b2e-102">Global and SharePoint admin</span></span>

<span data-ttu-id="45b2e-103">ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint ต้องได้รับการมอบหมายสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="45b2e-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="45b2e-104">บัญชีที่สร้างขึ้นใหม่ที่เพิ่งมอบหมายด้วยสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจพบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="45b2e-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="45b2e-105">โปรดให้เวลาอย่างน้อย 24 ชั่วโมงเพื่อให้การซิงค์เสร็จสมบูรณ์ระหว่างระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="45b2e-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="45b2e-106">เราเข้าใจว่าเวลา 24 ชั่วโมงอาจดูเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="45b2e-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="45b2e-107">ในหลายกรณี เราแก้ไขปัญหาเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="45b2e-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="45b2e-108">ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบส่วนกลางหรือ SharePoint มีสิทธิ์เข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") ระบุผู้ดูแลระบบไซต์ จัดการการตั้งค่าการแชร์ และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="45b2e-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="45b2e-109">พวกเขาไม่มีการเข้าถึงโดยอัตโนมัติไปยังไซต์ทั้งหมดและ OneDrive ของผู้ใช้แต่ละคน แต่พวกเขาสามารถให้ตนเองเข้าถึงไซต์หรือ OneDrive ได้</span><span class="sxs-lookup"><span data-stu-id="45b2e-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="45b2e-110">พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="45b2e-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="45b2e-111">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)</span><span class="sxs-lookup"><span data-stu-id="45b2e-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="45b2e-112">มีหลายสาเหตุที่ Microsoft SharePoint หรือ Microsoft OneDrive อาจไม่สามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="45b2e-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="45b2e-113">ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คู่มือต่อไปนี้เพื่อแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="45b2e-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="45b2e-114">ไม่สามารถเข้าถึง SharePoint Online ได้</span><span class="sxs-lookup"><span data-stu-id="45b2e-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [<span data-ttu-id="45b2e-115">การเข้าถึงถูกปฏิเสธบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive</span><span class="sxs-lookup"><span data-stu-id="45b2e-115">Access denied for PIM-managed user accounts in SharePoint or OneDrive admin center</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)