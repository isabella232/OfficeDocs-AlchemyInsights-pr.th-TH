---
title: ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421093"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="b5f74-102">ตัวจัดการ EndPoint - ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="b5f74-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="b5f74-103">ข้อมูลพื้นฐานเกี่ยวกับความปลอดภัยคือกลุ่มการตั้งค่า Windows ที่กําหนดค่าไว้ล่วงหน้า ซึ่งช่วยให้คุณปรับใช้การตั้งค่าความปลอดภัยที่แนะนาโดยทีมรักษาความปลอดภัยที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="b5f74-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="b5f74-104">ข้อมูลพื้นฐานเหล่านี้สามารถถูกปรับแต่งเพื่อให้แสดงเฉพาะการตั้งค่าและค่าที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="b5f74-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="b5f74-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices intuns](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="b5f74-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="b5f74-106">ขณะนี้มีข้อมูลพื้นฐานเกี่ยวกับผลิตภัณฑ์เหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="b5f74-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="b5f74-107">การตั้งค่าความปลอดภัยของ Windows MDM</span><span class="sxs-lookup"><span data-stu-id="b5f74-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="b5f74-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="b5f74-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="b5f74-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b5f74-109">Microsoft Edge</span></span>

<span data-ttu-id="b5f74-110">ข้อมูลพื้นฐานแต่ละรายการจะได้รับการอัปเดตเป็นระยะๆ และเผยแพร่ในเวอร์ชันที่เพิ่มขึ้น</span><span class="sxs-lookup"><span data-stu-id="b5f74-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="b5f74-111">แต่ละเวอร์ชันจะเพิ่มหรือนําการตั้งค่าออกจากเวอร์ชันก่อนหน้าเพื่อให้แน่ใจว่าข้อมูลพื้นฐานตรงตามแนวทางปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="b5f74-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="b5f74-112">คอนโซลข้อมูลพื้นฐานด้านความปลอดภัยในการรักษาความปลอดภัยของจุดสิ้นสุดช่วยให้สามารถเปรียบเทียบเวอร์ชันต่างๆ ได้โดยการเปลี่ยนแปลงจากเวอร์ชันสู่เวอร์ชันที่มองเห็นได้</span><span class="sxs-lookup"><span data-stu-id="b5f74-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="b5f74-113">สําหรับแนวทางเกี่ยวกับวิธีการเปลี่ยนอย่างมีประสิทธิภาพที่สุดว่าเวอร์ชันของแผนพื้นฐานมีการปรับใช้อย่างไร ให้ดู จัดการ[โปรไฟล์พื้นฐานด้านความปลอดภัยใน Microsoft Intuny](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="b5f74-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="b5f74-114">หลังจากการปรับใช้ข้อมูลพื้นฐานด้านความปลอดภัย คุณสามารถตรวจสอบสถานะของการปรับใช้และการตั้งค่าการตรวจสอบบนอุปกรณ์พื้นฐานได้</span><span class="sxs-lookup"><span data-stu-id="b5f74-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="b5f74-115">**หมายเหตุ:** ข้อมูลการรายงานของข้อมูลขั้นต้นอาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้ปรากฏจากการปรับใช้ครั้งแรกไปยังอุปกรณ์และสูงสุด 6 ชั่วโมงเพื่อการอัปเดตเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="b5f74-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="b5f74-116">สาเหตุทั่วไปของการตั้งค่าข้อมูลพื้นฐานที่ไม่ได้ใช้คือเพราะการตั้งค่าเดียวกันที่ใช้ในโปรไฟล์อื่น</span><span class="sxs-lookup"><span data-stu-id="b5f74-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="b5f74-117">สถานการณ์นี้สามารถตรวจสอบอุปกรณ์ที่เฉพาะเจาะจงได้โดยการเลือกอุปกรณ์นั้นจากภายในโหนดสถานะอุปกรณ์ของโปรไฟล์ข้อมูลพื้นฐานด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="b5f74-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="b5f74-118">For details, see [resolve conflicts for security baselines.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="b5f74-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>