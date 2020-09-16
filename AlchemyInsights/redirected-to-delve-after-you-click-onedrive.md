---
title: OneDrive for Business Web OneDrive เปลี่ยนเส้นทางไปยัง Delve
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776399"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="55efd-102">เปลี่ยนเส้นทางไปยัง Delve หลังจากที่คุณคลิก OneDrive</span><span class="sxs-lookup"><span data-stu-id="55efd-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="55efd-103">ดู [คำแนะนำการแก้ไขปัญหา](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)โดยละเอียดของเรา</span><span class="sxs-lookup"><span data-stu-id="55efd-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="55efd-104">เมื่อต้องการแก้ไขปัญหานี้ผู้ดูแลระบบต้องให้สิทธิ์ผู้ใช้ในการสร้างไซต์ไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="55efd-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="55efd-105">นี่คือเนื่องจากหน้า OneDrive for Business จะถูกสร้างขึ้นบนไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="55efd-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="55efd-106">เมื่อต้องการให้สิทธิ์นี้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="55efd-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="55efd-107">ในศูนย์การจัดการ SharePoint ให้คลิก**โปรไฟล์ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="55efd-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="55efd-108">ในส่วน**บุคคล**ให้คลิก**จัดการสิทธิ์ของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="55efd-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="55efd-109">เพิ่มผู้ใช้ที่จำเป็นต้องมีสิทธิ์ในการสร้างไซต์ไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="55efd-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="55efd-110">ตามค่าเริ่มต้นการตั้งค่านี้จะถูกตั้งค่าให้**ทุกคนยกเว้นผู้ใช้ภายนอก**</span><span class="sxs-lookup"><span data-stu-id="55efd-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="55efd-111">หลังจากที่คุณเพิ่มผู้ใช้ผู้ใช้หรือกลุ่มตรวจสอบให้แน่ใจว่าได้เลือกผู้ใช้ผู้ใช้หรือกลุ่มที่เพิ่มเข้าไปแล้วให้เลื่อนไปที่ส่วน**สิทธิ์**จากนั้นเลือกกล่องกาเครื่องหมายที่อยู่ถัดจาก**สร้างไซต์ส่วนบุคคล (จำเป็นต้องใช้สำหรับที่เก็บข้อมูลส่วนบุคคลตัวดึงข้อมูลข่าวสารและเนื้อหาที่ติดตาม)**</span><span class="sxs-lookup"><span data-stu-id="55efd-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="55efd-112">คลิก **ตกลง**จากนั้นให้ผู้ใช้เรียกดูไปยังหน้า OneDrive เพื่อสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="55efd-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
