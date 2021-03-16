---
title: เอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816340"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="a18f3-102">เอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก</span><span class="sxs-lookup"><span data-stu-id="a18f3-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="a18f3-103">เมื่อต้องการเอาบริการพื้นหลังของ Microsoft Search ใน Bing ออก คุณสามารถลองวิธีแก้ไขต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a18f3-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="a18f3-104">เมื่อต้องการย้อนกลับไปยังการตั้งค่าโปรแกรมค้นหาดั้งเดิม ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a18f3-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="a18f3-105">a.</span><span class="sxs-lookup"><span data-stu-id="a18f3-105">a.</span></span> <span data-ttu-id="a18f3-106">สลับ **ปุ่มปิดใช้ Bing เป็น [เครื่องมือค้นหาเริ่มต้น](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)** ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a18f3-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="a18f3-107">b.</span><span class="sxs-lookup"><span data-stu-id="a18f3-107">b.</span></span> <span data-ttu-id="a18f3-108">[ไปที่ศูนย์การจัดการ Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) และล้างการตั้งค่าที่มีผลต่อผู้ใช้ทุกคนในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="a18f3-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="a18f3-109">เมื่อต้องการเอาบริการพื้นหลังออกจากอุปกรณ์แต่ละเครื่อง ให้งานต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a18f3-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="a18f3-110">a.</span><span class="sxs-lookup"><span data-stu-id="a18f3-110">a.</span></span> <span data-ttu-id="a18f3-111">เลือก **แผงควบคุม >โปรแกรม>และฟีเจอร์**</span><span class="sxs-lookup"><span data-stu-id="a18f3-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="a18f3-112">b.</span><span class="sxs-lookup"><span data-stu-id="a18f3-112">b.</span></span> <span data-ttu-id="a18f3-113">คลิกขวาที่ **Microsoft Search ใน Bing** ภายใต้รายการโปรแกรมที่ติดตั้ง **แล้วคลิก** ถอนการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="a18f3-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="a18f3-114">เมื่อต้องการเอาบริการพื้นหลังออกจากอุปกรณ์หลายเครื่องในองค์กรของคุณ ให้เข้าสู่ระบบในฐานะผู้ดูแลระบบ และเรียกใช้สั่งต่อไปนี้ในสคริปต์:</span><span class="sxs-lookup"><span data-stu-id="a18f3-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
