---
title: การเข้าถึงแบบมีเงื่อนไขกับ Intun
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931455"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="07e02-102">การเข้าถึงแบบมีเงื่อนไขกับ Intun</span><span class="sxs-lookup"><span data-stu-id="07e02-102">Conditional Access with Intune</span></span>

<span data-ttu-id="07e02-103">การใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intunเน จําเป็นต้องมีขั้นตอนที่ 3:</span><span class="sxs-lookup"><span data-stu-id="07e02-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="07e02-104">สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกําหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าเป็นไปตาม</span><span class="sxs-lookup"><span data-stu-id="07e02-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="07e02-105">ตัวอย่างเช่น อุปกรณ์ต้องมีหมุดอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามข้อกําหนด</span><span class="sxs-lookup"><span data-stu-id="07e02-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="07e02-106">สร้าง**นโยบายการเข้าถึงแบบมีเงื่อนไข**ที่กําหนดทรัพยากรที่ถูกป้องกัน และต้องเป็นไปตามเงื่อนไขใดเพื่อเข้าถึงทรัพยากรเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="07e02-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="07e02-107">[ตัวอย่างเช่น](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)อุปกรณ์ต้องเป็นไปตามข้อกําหนดก่อนที่จะเข้าถึงอีเมลขององค์กร</span><span class="sxs-lookup"><span data-stu-id="07e02-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="07e02-108">ตรวจสอบให้แน่ใจว่านโยบาย**การปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงตามเงื่อนไข**ถูกกําหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="07e02-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="07e02-109">ซึ่งอาจต้องใช้การสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="07e02-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="07e02-110">**การเชื่อมโยงที่เป็นประโยชน์:**</span><span class="sxs-lookup"><span data-stu-id="07e02-110">**Helpful links:**</span></span>

[<span data-ttu-id="07e02-111">ภาพรวมการปฏิบัติตามข้อกําหนดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="07e02-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="07e02-112">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="07e02-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="07e02-113">นโยบายการแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="07e02-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="07e02-114">เมื่อต้องการป้องกันอีเมล (Exchange แบบออนไลน์) จากการเข้าถึง โดยอุปกรณ์ที่ไม่ปฏิบัติตาม เอกสารทั้งสองต้องปฏิบัติตาม:</span><span class="sxs-lookup"><span data-stu-id="07e02-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="07e02-115">ปกป้องการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ EAS</span><span class="sxs-lookup"><span data-stu-id="07e02-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="07e02-116">ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ไคลเอ็นต์การรับรองความถูกต้องแบบสมัยใหม่เช่น Outlook</span><span class="sxs-lookup"><span data-stu-id="07e02-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)