---
title: เพิ่ม Microsoft Edge ไปยัง Microsoft Intun1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194578"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="968f6-102">เพิ่ม Microsoft Edge ไปยัง Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="968f6-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="968f6-103">เพื่อให้สามารถปรับใช้ กําหนดค่า ตรวจสอบ และปกป้อง Microsoft Edge for Windows 10 ได้ คุณต้องเพิ่ม Microsoft Intuned ก่อน</span><span class="sxs-lookup"><span data-stu-id="968f6-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="968f6-104">Intun1 สนับสนุน Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="968f6-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="968f6-105">Intuned จะตรวจหาการติดตั้ง Microsoft Edge ที่มีอยู่ก่อน</span><span class="sxs-lookup"><span data-stu-id="968f6-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="968f6-106">ถ้า Microsoft Edge ถูกติดตั้งในบริบทของผู้ใช้ การติดตั้งระบบจะเขียนทับการติดตั้งในบริบทของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="968f6-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="968f6-107">ถ้า Microsoft Edge ได้รับการติดตั้งในบริบทของระบบ ระบบจะรายงานความสเร็จในการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="968f6-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="968f6-108">Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่าที่ติดตั้งไว้ล่วงหน้าในแชนเนลทั้งหมดในบริบทของผู้ใช้จะถูกเขียนทับด้วย Microsoft Edge ที่ติดตั้งในบริบทของระบบ</span><span class="sxs-lookup"><span data-stu-id="968f6-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="968f6-109">**เงื่อนไขเบื้องต้น**</span><span class="sxs-lookup"><span data-stu-id="968f6-109">**Prerequisite**</span></span>

<span data-ttu-id="968f6-110">Windows 10 เวอร์ชัน 1709 หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="968f6-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="968f6-111">**ขั้นตอนในการเพิ่ม Edge ไปยัง Intuned**</span><span class="sxs-lookup"><span data-stu-id="968f6-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="968f6-112">[กําหนดค่าแอปใน Intun>](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="968f6-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="968f6-113">[กําหนดค่าข้อมูล](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป</span><span class="sxs-lookup"><span data-stu-id="968f6-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="968f6-114">[กําหนดค่าการตั้งค่า](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป</span><span class="sxs-lookup"><span data-stu-id="968f6-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="968f6-115">[เลือกแท็กขอบเขต (ไม่บังคับ)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="968f6-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="968f6-116">[เพิ่ม](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป</span><span class="sxs-lookup"><span data-stu-id="968f6-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="968f6-117">หากต้องการความช่วยเหลือเพิ่มเติม [โปรดดู](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)การแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="968f6-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




