---
title: สร้างกลุ่ม
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816391"
---
# <a name="create-a-group"></a><span data-ttu-id="70480-102">สร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="70480-102">Create a group</span></span>

<span data-ttu-id="70480-103">หัวข้อนี้จะอธิบายเกี่ยวกับการสร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="70480-103">This topic describes group creation.</span></span>

<span data-ttu-id="70480-104">**สิทธิ์ในการสร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="70480-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="70480-105">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่</span><span class="sxs-lookup"><span data-stu-id="70480-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="70480-106">ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัล Azure หรือแผงการเข้าถึงได้</span><span class="sxs-lookup"><span data-stu-id="70480-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="70480-107">คุณอาจต้องใช้ผู้ดูแลระบบเพื่อสร้างกลุ่มใหม่ให้คุณ หรือมอบสิทธิ์ที่เหมาะสมแก่คุณ</span><span class="sxs-lookup"><span data-stu-id="70480-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="70480-108">**จัดการสิทธิ์การสร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="70480-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="70480-109">ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การสร้างกลุ่ม (ด้วยเหตุผลด้านความปลอดภัย) หรือกลุ่ม Office 365 ที่สร้างขึ้นในพอร์ทัล Azure หรือแผงการเข้าถึง โดยเลือก "ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล Azure" หรือ "ผู้ใช้สามารถสร้างกลุ่ม Office 365 ในพอร์ทัลAzure" ใน ตัวเลือก กลุ่มทั้งหมด  >  **ทั่วไป (การตั้งค่า)**</span><span class="sxs-lookup"><span data-stu-id="70480-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="70480-110">คุณยังสามารถจํากัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ ถ้าคุณมีสิทธิ์การใช้งาน Azure Active Directory P1 Premium</span><span class="sxs-lookup"><span data-stu-id="70480-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="70480-111">**การปิดใช้งานการแจ้งเตือนต้อนรับของสมาชิกกลุ่ม Office 365 ใหม่**</span><span class="sxs-lookup"><span data-stu-id="70480-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="70480-112">การแจ้งเตือนต้อนรับที่ส่งถึงผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office 365 สามารถถูกปิดใช้งานโดยการตั้งค่า **UnifiedGroupWelcomesMessageEnabled** เป็น False ใน Powershell</span><span class="sxs-lookup"><span data-stu-id="70480-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="70480-113">เรียนรู้เกี่ยวกับการตั้งค่า [นี้](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)ที่นี่</span><span class="sxs-lookup"><span data-stu-id="70480-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

