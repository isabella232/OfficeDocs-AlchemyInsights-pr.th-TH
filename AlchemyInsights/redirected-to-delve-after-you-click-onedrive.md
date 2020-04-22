---
title: การเปลี่ยนเส้นทางไปยัง Delve สําหรับธุรกิจเว็บ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722829"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="2d3e5-102">เปลี่ยนเส้นทางไปยัง Delve หลังจากที่คุณคลิก OneDrive</span><span class="sxs-lookup"><span data-stu-id="2d3e5-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="2d3e5-103">ดู[รายละเอียดของเรา](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="2d3e5-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="2d3e5-104">เมื่อต้องการแก้ไขปัญหานี้ ผู้ดูแลต้องให้สิทธิ์แก่ผู้ใช้ในการสร้างไซต์ไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="2d3e5-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="2d3e5-105">นี่คือเนื่องจากหน้า OneDrive สําหรับธุรกิจถูกสร้างขึ้นบนไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="2d3e5-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="2d3e5-106">เมื่อต้องการให้สิทธิ์นี้ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="2d3e5-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="2d3e5-107">ใน ศูนย์การจัดการ SharePoint ให้คลิก**โพรไฟล์ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="2d3e5-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="2d3e5-108">ในส่วน**บุคคล**ให้คลิก**จัดการสิทธิ์ของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="2d3e5-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="2d3e5-109">เพิ่มผู้ใช้ที่ต้องการสิทธิ์เพื่อสร้างไซต์ไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="2d3e5-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="2d3e5-110">การตั้งค่านี้จะถูกตั้งค่าเป็น**ทุกคน ยกเว้น ผู้ใช้ภายนอก**</span><span class="sxs-lookup"><span data-stu-id="2d3e5-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="2d3e5-111">หลังจากที่คุณได้เพิ่มผู้ใช้ ผู้ใช้ หรือกลุ่ม แล้ว ตรวจสอบให้แน่ใจว่าผู้ใช้ ผู้ใช้ หรือกลุ่มที่ถูกเพิ่มถูกเลือก แล้วเลื่อนไปที่ส่วน**สิทธิ์**แล้วเลือกกล่องกาเครื่องหมายที่อยู่ถัดจาก**สร้างไซต์ส่วนบุคคล (จําเป็นสําหรับที่เก็บข้อมูลส่วนบุคคล ตัวดึงข้อมูลข่าวสาร และเนื้อหาตามด้วย)**</span><span class="sxs-lookup"><span data-stu-id="2d3e5-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="2d3e5-112">คลิก**ตกลง**แล้วให้ผู้ใช้เรียกดูเพจ OneDrive เพื่อสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="2d3e5-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
