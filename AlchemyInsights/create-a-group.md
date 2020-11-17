---
title: สร้างกลุ่ม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089178"
---
# <a name="create-a-group"></a><span data-ttu-id="80eed-102">สร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="80eed-102">Create a group</span></span>

<span data-ttu-id="80eed-103">หัวข้อนี้จะอธิบายเกี่ยวกับการสร้างกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="80eed-103">This topic describes group creation.</span></span>

<span data-ttu-id="80eed-104">**สิทธิ์ในการสร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="80eed-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="80eed-105">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่</span><span class="sxs-lookup"><span data-stu-id="80eed-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="80eed-106">ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัลไซต์ Azure หรือแผงการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="80eed-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="80eed-107">คุณอาจจำเป็นต้องมีผู้ดูแลระบบในการสร้างกลุ่มใหม่ให้กับคุณหรือเพื่อให้สิทธิ์ที่เหมาะสมกับคุณ</span><span class="sxs-lookup"><span data-stu-id="80eed-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="80eed-108">**จัดการสิทธิ์ในการสร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="80eed-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="80eed-109">ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์ในการสร้างกลุ่มได้ (สำหรับเหตุผลด้านความปลอดภัย) หรือกลุ่ม Office ๓๖๕ที่สร้างขึ้นในพอร์ทัล azure หรือแผงการเข้าถึงโดยการเลือก "ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล azure" หรือ "ผู้ใช้สามารถสร้างกลุ่ม Office ๓๖๕ในพอร์ทัลไซต์ azure" ได้ในตัวเลือกใน **กลุ่ม**  >  **ทั่วไป (การตั้งค่า)**</span><span class="sxs-lookup"><span data-stu-id="80eed-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="80eed-110">นอกจากนี้คุณยังสามารถจำกัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ถ้าคุณมีสิทธิ์การใช้งาน Azure ของไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="80eed-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="80eed-111">**การปิดใช้งานการแจ้งให้ทราบยินดีต้อนรับสำหรับสมาชิกกลุ่ม Office ๓๖๕ใหม่**</span><span class="sxs-lookup"><span data-stu-id="80eed-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="80eed-112">การแจ้งเตือนยินดีต้อนรับที่ส่งไปยังผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office ๓๖๕สามารถปิดใช้งานได้โดยการตั้งค่า **UnifiedGroupWelcomeMessageEnabled** เป็น False ใน Powershell</span><span class="sxs-lookup"><span data-stu-id="80eed-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="80eed-113">เรียนรู้เกี่ยวกับการตั้งค่านี้[ที่นี่](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="80eed-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

