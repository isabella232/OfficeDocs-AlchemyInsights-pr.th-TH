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
ms.openlocfilehash: c39fec48f791d5cc4a97688cc7b5cd93010403a2
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791277"
---
# <a name="enrolling-android-devices-into-intune"></a><span data-ttu-id="2e821-102">การลงทะเบียนอุปกรณ์ Android ลงใน Intune</span><span class="sxs-lookup"><span data-stu-id="2e821-102">Enrolling Android devices into Intune</span></span>

<span data-ttu-id="2e821-103">ถ้าคุณกำลังมองหาการโยกย้ายผู้ใช้จากการลงทะเบียนผู้ดูแลระบบอุปกรณ์ Android ไปยัง Android Enterprise โปรดตรวจทาน:[ย้ายอุปกรณ์ Android จากผู้ดูแลระบบอุปกรณ์ไปยังการจัดการโปรไฟล์การทำงาน](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile)</span><span class="sxs-lookup"><span data-stu-id="2e821-103">If you are looking to migrate users from Android Device Administrator enrollment to Android Enterprise, please review: [Move Android devices from device administrator to work profile management](https://docs.microsoft.com/mem/intune/enrollment/android-move-device-admin-work-profile).</span></span>

<span data-ttu-id="2e821-104">Intune สนับสนุนการลงทะเบียนอุปกรณ์ Android ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="2e821-104">Intune supports the enrollment of the following Android devices:</span></span>  

- [<span data-ttu-id="2e821-105">ซัมซุง Knox, ม้าลาย, ผู้ดูแลระบบอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="2e821-105">Samsung Knox, Zebra, Device Administrator</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enroll-device-administrator)
- [<span data-ttu-id="2e821-106">โปรไฟล์การทำงานขององค์กร Android</span><span class="sxs-lookup"><span data-stu-id="2e821-106">Android Enterprise work profile</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-enterprise-overview)
- [<span data-ttu-id="2e821-107">Android Enterprise ที่ทุ่มเท</span><span class="sxs-lookup"><span data-stu-id="2e821-107">Android Enterprise dedicated</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-dedicated-devices-fully-managed-enroll)
- [<span data-ttu-id="2e821-108">Android Enterprise ที่มีการจัดการทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="2e821-108">Android Enterprise fully managed</span></span>](https://docs.microsoft.com/mem/intune/enrollment/android-fully-managed-enroll)

<span data-ttu-id="2e821-109">ก่อนที่จะตั้งค่าการลงทะเบียนสำหรับอุปกรณ์ Android ให้[ตรวจทานก่อน requisites](https://docs.microsoft.com/intune/enrollment/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="2e821-109">Before setting up enrollment for Android devices, [review the pre-requisites](https://docs.microsoft.com/intune/enrollment/android-enroll).</span></span>  

<span data-ttu-id="2e821-110">สำหรับข้อมูลเกี่ยวกับการแก้ไขปัญหาการลงทะเบียนอุปกรณ์ในทั่วไปและข้อผิดพลาดการลงทะเบียน Android บางรายการให้ดูที่การ[แก้ไขปัญหาการลงทะเบียนอุปกรณ์ใน Microsoft Intune](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment)</span><span class="sxs-lookup"><span data-stu-id="2e821-110">For information on troubleshooting device enrollment in general and some Android enrollment errors, see [Troubleshoot device enrollment in Microsoft Intune](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-android-enrollment).</span></span>

<span data-ttu-id="2e821-111">นอกจากนี้คุณยังสามารถใช้เนื้อหาที่อธิบายถึงใบมีดการแก้ไขปัญหาของ Intune เพื่อช่วยระบุว่าปัญหาการลงทะเบียนผู้ใช้ของคุณประสบปัญหาอะไรบ้าง</span><span class="sxs-lookup"><span data-stu-id="2e821-111">You can also use the content describing the Intune Troubleshooting blade to help identify what enrolment issues your users are experiencing.</span></span>
