---
title: ผู้ดูแลระบบส่วนกลางและ SharePoint
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
- "9002962"
- "5674"
ms.openlocfilehash: 9d4c5da8b6dc78aa18fd29589495b77b7d835aba
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706394"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="189bd-102">ผู้ดูแลระบบส่วนกลางและ SharePoint</span><span class="sxs-lookup"><span data-stu-id="189bd-102">Global and SharePoint admin</span></span>

<span data-ttu-id="189bd-103">ผู้ดูแลระบบส่วนกลางและผู้ดูแลระบบ SharePoint จำเป็นต้องได้รับการกำหนดสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="189bd-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="189bd-104">บัญชีผู้ใช้ที่สร้างขึ้นใหม่เพิ่งมอบหมายให้กับสิทธิ์การใช้งาน SharePoint หรือบทบาทผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "access denied" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="189bd-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="189bd-105">โปรดให้การซิงค์อย่างน้อย24ชั่วโมงเพื่อให้เสร็จสมบูรณ์ในระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="189bd-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="189bd-106">เราเข้าใจว่า24ชั่วโมงอาจดูเหมือนเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="189bd-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="189bd-107">ในหลายกรณีเรากำลังทำงานกับโซลูชันอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="189bd-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="189bd-108">ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบส่วนกลางหรือ SharePoint จะมีสิทธิ์เข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ได้ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน") ที่กำหนดผู้ดูแลไซต์จัดการการตั้งค่าการแชร์และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="189bd-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="189bd-109">พวกเขาไม่มีการเข้าถึงไซต์ทั้งหมดโดยอัตโนมัติและ OneDrive ของผู้ใช้แต่ละคนแต่พวกเขาสามารถให้สิทธิ์การเข้าถึงไซต์หรือ OneDrive ของผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="189bd-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="189bd-110">นอกจากนี้พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive ได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="189bd-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="189bd-111">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดู[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft ๓๖๕](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)</span><span class="sxs-lookup"><span data-stu-id="189bd-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="189bd-112">มีเหตุผลหลายประการที่ Microsoft SharePoint หรือ Microsoft OneDrive อาจไม่สามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="189bd-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="189bd-113">ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คำแนะนำต่อไปนี้เพื่อแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="189bd-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="189bd-114">ไม่สามารถเข้าถึง SharePoint Online ได้</span><span class="sxs-lookup"><span data-stu-id="189bd-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [<span data-ttu-id="189bd-115">การเข้าถึงถูกปฏิเสธสำหรับบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive</span><span class="sxs-lookup"><span data-stu-id="189bd-115">Access denied for PIM-managed user accounts in SharePoint or OneDrive admin center</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)