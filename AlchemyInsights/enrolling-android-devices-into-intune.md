---
title: การลงทะเบียนอุปกรณ์ Android ลงใน Intune
ms.author: erikje
author: erikje
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "2494"
ms.openlocfilehash: 9306f56e2f3b9ba3b06e78e07aa2eb0fe40817e4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784326"
---
# <a name="enrolling-android-devices-into-intune"></a><span data-ttu-id="7d7d8-102">การลงทะเบียนอุปกรณ์ Android ลงใน Intune</span><span class="sxs-lookup"><span data-stu-id="7d7d8-102">Enrolling Android devices into Intune</span></span>

<span data-ttu-id="7d7d8-103">Intune สนับสนุนการลงทะเบียนอุปกรณ์ Android ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7d7d8-103">Intune supports the enrollment of the following Android devices:</span></span>
- <span data-ttu-id="7d7d8-104">ซัมซุง Knox และม้าลาย</span><span class="sxs-lookup"><span data-stu-id="7d7d8-104">Samsung Knox and Zebra</span></span>
- <span data-ttu-id="7d7d8-105">โปรไฟล์การทำงานขององค์กร Android</span><span class="sxs-lookup"><span data-stu-id="7d7d8-105">Android Enterprise work profile</span></span>
- <span data-ttu-id="7d7d8-106">Android Enterprise ที่ทุ่มเท</span><span class="sxs-lookup"><span data-stu-id="7d7d8-106">Android Enterprise dedicated</span></span>
- <span data-ttu-id="7d7d8-107">Android Enterprise ที่มีการจัดการทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="7d7d8-107">Android Enterprise fully managed</span></span>

<span data-ttu-id="7d7d8-108">ก่อนที่จะตั้งค่าการลงทะเบียนสำหรับอุปกรณ์ Android [ตรวจทานก่อน-requisites https://docs.microsoft.com/intune/enrollment/android-enroll ] (</span><span class="sxs-lookup"><span data-stu-id="7d7d8-108">Before setting up enrollment for Android devices, [review the pre-requisites](https://docs.microsoft.com/intune/enrollment/android-enroll.</span></span>

<span data-ttu-id="7d7d8-109">สำหรับข้อมูลเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนอุปกรณ์ในทั่วไปและข้อผิดพลาดการลงทะเบียน Android บางรายการให้ดูที่การ[แก้ไขปัญหาการลงทะเบียนอุปกรณ์ใน Microsoft Intune](https://docs.microsoft.com/intune/enrollment/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7d7d8-109">For information on troubleshooting device enrollment in general and some Android enrollment errors,  see [Troubleshoot device enrollment in Microsoft Intune](https://docs.microsoft.com/intune/enrollment/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="7d7d8-110">นอกจากนี้คุณยังสามารถใช้ [เนื้อหาที่อธิบายถึงใบมีดการแก้ไขปัญหาของ Intune](https://docs.microsoft.com/intune/fundamentals/help-desk-operators) เพื่อช่วยระบุว่าปัญหาการลงทะเบียนผู้ใช้ของคุณประสบปัญหาอะไรบ้าง</span><span class="sxs-lookup"><span data-stu-id="7d7d8-110">You can also use the [content describing the Intune Troubleshooting blade](https://docs.microsoft.com/intune/fundamentals/help-desk-operators) to help identify what enrolment issues your users are experiencing.</span></span>





