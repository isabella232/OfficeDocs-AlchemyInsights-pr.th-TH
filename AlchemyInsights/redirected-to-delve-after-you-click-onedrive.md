---
title: OneDrive for Business Web OneDrive เปลี่ยนเส้นทางไปยัง Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800008"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="f7321-102">เปลี่ยนเส้นทางไปยัง Delve หลังจากที่คุณคลิก OneDrive</span><span class="sxs-lookup"><span data-stu-id="f7321-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="f7321-103">ดูคู่มือ [การแก้ไขปัญหาโดยละเอียด](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)ของเรา</span><span class="sxs-lookup"><span data-stu-id="f7321-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="f7321-104">เมื่อต้องการแก้ไขปัญหานี้ ผู้ดูแลระบบต้องมอบสิทธิ์ในการสร้างไซต์ไซต์ของฉันให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f7321-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="f7321-105">เนื่องจากหน้า OneDrive for Business ถูกสร้างขึ้นบนไซต์ของฉัน</span><span class="sxs-lookup"><span data-stu-id="f7321-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="f7321-106">เมื่อต้องการให้สิทธิ์นี้ ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f7321-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="f7321-107">ในศูนย์การจัดการ SharePoint **ให้คลิก โปรไฟล์** ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f7321-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="f7321-108">ในส่วน **บุคคล** ให้คลิก **จัดการสิทธิ์ของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="f7321-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="f7321-109">เพิ่มผู้ใช้ที่ต้องใช้สิทธิ์ในการสร้างไซต์ไซต์ของฉันของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="f7321-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="f7321-110">ตามค่าเริ่มต้น การตั้งค่านี้จะถูกตั้งค่า **เป็น ทุกคน ยกเว้นผู้ใช้** ภายนอก</span><span class="sxs-lookup"><span data-stu-id="f7321-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="f7321-111">หลังจากที่คุณเพิ่มผู้ใช้ ผู้ใช้ หรือกลุ่มแล้ว ตรวจสอบให้แน่ใจว่าได้เลือก ผู้ใช้ ผู้ใช้ หรือกลุ่มที่เพิ่มแล้ว ให้เลื่อนไปยังส่วนสิทธิ์ แล้วเลือกกล่องกาเครื่องหมายที่อยู่ถัดจาก สร้างไซต์ส่วนบุคคล (ต้องใช้กับที่เก็บส่วนบุคคล ตัวดึงข้อมูลข่าวสาร และเนื้อหาที่ **ติดตาม)**</span><span class="sxs-lookup"><span data-stu-id="f7321-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="f7321-112">**คลิก** ตกลง แล้วให้ผู้ใช้เรียกดูหน้า OneDrive เพื่อสร้างไซต์</span><span class="sxs-lookup"><span data-stu-id="f7321-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
