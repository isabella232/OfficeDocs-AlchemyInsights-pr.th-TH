---
title: OneDrive สำหรับ OneDrive ธุรกิจเว็บเปลี่ยนเส้นทางไปยัง Delve
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
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571254"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="cdd9b-102">เปลี่ยนเส้นทางไปยัง Delve หลังจากที่คุณคลิก OneDrive</span><span class="sxs-lookup"><span data-stu-id="cdd9b-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="cdd9b-103">ดู[คู่มือการแก้ไขปัญหา](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)โดยละเอียดของเรา</span><span class="sxs-lookup"><span data-stu-id="cdd9b-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="cdd9b-104">เมื่อต้องการแก้ไขปัญหานี้ผู้ดูแล Office ๓๖๕ต้องให้สิทธิ์ผู้ใช้ในการสร้างไซต์ของฉันไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="cdd9b-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="cdd9b-105">นี่คือเนื่องจากการ OneDrive สำหรับหน้าธุรกิจถูกสร้างขึ้นบนไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="cdd9b-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="cdd9b-106">เมื่อต้องการให้สิทธิ์นี้ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="cdd9b-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="cdd9b-107">ในศูนย์ดูแล SharePoint คลิก**โพรไฟล์ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="cdd9b-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="cdd9b-108">ในการ**บุคคล**ส่วนคลิ**กจัดการสิทธิ์ของผู้ใช้**.</span><span class="sxs-lookup"><span data-stu-id="cdd9b-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="cdd9b-109">เพิ่มผู้ใช้ที่จำเป็นต้องมีสิทธิ์ในการสร้างไซต์ของฉันไซต์</span><span class="sxs-lookup"><span data-stu-id="cdd9b-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="cdd9b-110">โดยค่าเริ่มต้นการตั้งค่านี้ถูกตั้งค่าให้**ทุกคนยกเว้นผู้ใช้ภายนอก**</span><span class="sxs-lookup"><span data-stu-id="cdd9b-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="cdd9b-111">หลังจากที่คุณได้เพิ่มผู้ใช้ผู้ใช้หรือกลุ่มให้ตรวจสอบให้แน่ใจว่าได้เลือกผู้ใช้ผู้ใช้หรือกลุ่มที่เพิ่มเข้าไปแล้วให้เลื่อนไปที่ส่วน**สิทธิ์**แล้วเลือกกล่องกาเครื่องหมายที่อยู่ถัดจาก**สร้างไซต์ส่วนบุคคล (จำเป็นสำหรับการเก็บข้อมูลส่วนบุคคล, สารดึงและการติดตามเนื้อหา)**</span><span class="sxs-lookup"><span data-stu-id="cdd9b-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="cdd9b-112">คลิ**กตกลง**และจากนั้นมีผู้ใช้เรียกดูไปยังหน้า OneDrive เพื่อสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="cdd9b-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
