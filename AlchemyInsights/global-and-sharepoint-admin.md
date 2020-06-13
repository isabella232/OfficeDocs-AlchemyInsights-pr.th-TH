---
title: ส่วนกลางและผู้ดูแลระบบ SharePoint
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: 231f302bd3f3655b1fe72518d71b14d464914ce0
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716438"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="9382a-102">ส่วนกลางและผู้ดูแลระบบ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9382a-102">Global and SharePoint admin</span></span>

<span data-ttu-id="9382a-103">ผู้ดูแลระบบส่วนกลางและ SharePoint ต้องได้รับมอบหมายสิทธิ์การใช้งาน SharePoint</span><span class="sxs-lookup"><span data-stu-id="9382a-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="9382a-104">บัญชีที่สร้างขึ้นใหม่เพิ่งได้รับมอบหมายด้วยบทบาทสิทธิ์การใช้งาน SharePoint หรือผู้ดูแลระบบอาจประสบปัญหาในการเข้าถึง SharePoint เช่น "การเข้าถึงถูกปฏิเสธ" หรือ "ไม่พบผู้ใช้"</span><span class="sxs-lookup"><span data-stu-id="9382a-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="9382a-105">โปรดให้อย่างน้อย 24 ชั่วโมงสําหรับการซิงค์เพื่อให้เสร็จสมบูรณ์ในระบบของเรา</span><span class="sxs-lookup"><span data-stu-id="9382a-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="9382a-106">เราเข้าใจว่า 24 ชั่วโมงอาจดูเหมือนเป็นเวลานาน</span><span class="sxs-lookup"><span data-stu-id="9382a-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="9382a-107">ในหลายกรณีเรากําลังทํางานอยู่แล้วในการแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="9382a-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="9382a-108">ผู้ใช้ที่ได้รับมอบหมายบทบาทผู้ดูแลระบบ Global หรือ SharePoint สามารถเข้าถึงศูนย์การจัดการ SharePoint และสามารถสร้างและจัดการไซต์ (ก่อนหน้านี้เรียกว่า "ไซต์คอลเลกชัน")</span><span class="sxs-lookup"><span data-stu-id="9382a-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="9382a-109">พวกเขาไม่มีการเข้าถึงโดยอัตโนมัติไปยังไซต์ทั้งหมดและ OneDrive ของผู้ใช้แต่ละราย แต่พวกเขาสามารถให้ตัวเองเข้าถึงเว็บไซต์หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9382a-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="9382a-110">นอกจากนี้ พวกเขายังสามารถใช้ Microsoft PowerShell เพื่อจัดการ SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9382a-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="9382a-111">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูที่[เกี่ยวกับบทบาทผู้ดูแลระบบ SharePoint ใน Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)</span><span class="sxs-lookup"><span data-stu-id="9382a-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="9382a-112">มีหลายสาเหตุที่ทําให้ Microsoft SharePoint หรือ Microsoft OneDrive ไม่สามารถเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="9382a-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="9382a-113">ถ้าคุณไม่สามารถเข้าถึง SharePoint Online ให้ใช้คําแนะนําต่อไปนี้เพื่อแก้ไขปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="9382a-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="9382a-114">ไม่สามารถเข้าถึง SharePoint แบบออนไลน์ได้</span><span class="sxs-lookup"><span data-stu-id="9382a-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [<span data-ttu-id="9382a-115">การเข้าถึงถูกปฏิเสธสําหรับบัญชีผู้ใช้ที่มีการจัดการ PIM ใน SharePoint หรือศูนย์การจัดการ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9382a-115">Access denied for PIM-managed user accounts in SharePoint or OneDrive admin center</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)