---
title: อัปเดตอุปกรณ์ iOS ไปยังเวอร์ชันล่าสุดของระบบปฏิบัติการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1124"
- "6700007"
ms.openlocfilehash: ee2fb1df35168d5febbac0ae302106eef9d1d18d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757643"
---
# <a name="update-ios-device-to-latest-os-version"></a><span data-ttu-id="0a8a9-102">อัปเดตอุปกรณ์ iOS ไปยังเวอร์ชันล่าสุดของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="0a8a9-102">Update iOS device to latest OS version</span></span>

<span data-ttu-id="0a8a9-103">การอัปเดตเวอร์ชันของระบบปฏิบัติการจะพร้อมใช้งานเฉพาะบนอุปกรณ์ที่มีการดูแลระบบและบนอุปกรณ์ iOS ที่ใช้ iOS ๑๐.๓และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="0a8a9-103">Operating system version updates are available only on supervised devices and on iOS devices running iOS 10.3 and later.</span></span>

<span data-ttu-id="0a8a9-104">ถ้าอุปกรณ์ของคุณมีคุณสมบัติตรงตามข้อกำหนดเวอร์ชันให้ตรวจสอบว่า:</span><span class="sxs-lookup"><span data-stu-id="0a8a9-104">If your devices meet the version requirements, verify that:</span></span>  
- <span data-ttu-id="0a8a9-105">ผู้ใช้อุปกรณ์ยังไม่ได้เลื่อนการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="0a8a9-105">Device users have not postponed updates.</span></span>  
- <span data-ttu-id="0a8a9-106">การตั้งค่านโยบายการอัปเดต iOS ปัจจุบันเช่นช่วงเวลาที่จำกัดจะไม่เป็นการป้องกันไม่ให้มีการติดตั้งการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="0a8a9-106">Current iOS update policy settings, such as restricted time periods, are not preventing updates from being installed.</span></span>

<span data-ttu-id="0a8a9-107">เมื่อต้องการอัปเดต iOS ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="0a8a9-107">To update your iOS:</span></span>

1. <span data-ttu-id="0a8a9-108">ลงชื่อเข้าใช้พอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="0a8a9-108">Sign in to the Azure portal.</span></span>
2. <span data-ttu-id="0a8a9-109">เลือก**บริการ Intune ทั้งหมด**  >  **Intune**</span><span class="sxs-lookup"><span data-stu-id="0a8a9-109">Choose **All services** > **Intune**.</span></span>
3. <span data-ttu-id="0a8a9-110">ในบานหน้าต่าง Intune ให้เลือก**Software updates**  >  **นโยบายการอัปเดตซอฟต์แวร์สำหรับ iOS**</span><span class="sxs-lookup"><span data-stu-id="0a8a9-110">In the Intune pane, choose **Software updates** > **Update policies for iOS**.</span></span>