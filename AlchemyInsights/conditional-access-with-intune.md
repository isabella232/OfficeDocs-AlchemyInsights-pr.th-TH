---
title: การเข้าถึงตามเงื่อนไขด้วย Intun1
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704805"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8a09d-102">การเข้าถึงตามเงื่อนไขด้วย Intun1</span><span class="sxs-lookup"><span data-stu-id="8a09d-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8a09d-103">การใช้  **การเข้าถึงตามเงื่อนไขด้วย**  Intun1 ต้องมี 3 ขั้นตอน:</span><span class="sxs-lookup"><span data-stu-id="8a09d-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="8a09d-104">สร้างนโยบาย  **การปฏิบัติตามนโยบาย**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว</span><span class="sxs-lookup"><span data-stu-id="8a09d-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="8a09d-105">ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าตรงตามมาตรฐาน</span><span class="sxs-lookup"><span data-stu-id="8a09d-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="8a09d-106">สร้าง **นโยบายการเข้าถึงตามเงื่อนไข**  ที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่ต้องใช้เพื่อเข้าถึงทรัพยากรเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="8a09d-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="8a09d-107">[ตัวอย่างเช่น อุปกรณ์](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  จะต้องปฏิบัติตามนโยบายก่อนที่จะเข้าถึงอีเมลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="8a09d-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="8a09d-108">ตรวจสอบให้แน่ใจ **ว่านโยบายการปฏิบัติตาม\*\*\*\*นโยบายและนโยบายการเข้าถึง** ตามเงื่อนไขถูกตั้งเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="8a09d-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="8a09d-109">ซึ่งอาจต้องมีการสร้างกลุ่มเฉพาะของผู้ใช้ใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8a09d-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="8a09d-110">**ลิงก์ที่เป็นประโยชน์:**</span><span class="sxs-lookup"><span data-stu-id="8a09d-110">**Helpful links:**</span></span>

[<span data-ttu-id="8a09d-111">ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="8a09d-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="8a09d-112">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="8a09d-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="8a09d-113">การแก้ไขปัญหานโยบาย</span><span class="sxs-lookup"><span data-stu-id="8a09d-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="8a09d-114">เมื่อต้องการป้องกันอีเมล (Exchange Online) จากการเข้าถึงด้วยอุปกรณ์ที่ไม่เข้ากัน ต้องปฏิบัติตามทั้งสองเอกสาร:</span><span class="sxs-lookup"><span data-stu-id="8a09d-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="8a09d-115">ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ EAS</span><span class="sxs-lookup"><span data-stu-id="8a09d-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="8a09d-116">ป้องกันการเข้าถึงอีเมลจากอุปกรณ์โดยใช้ไคลเอ็นต์การรับรองความถูกต้องสมัยใหม่ เช่น Outlook</span><span class="sxs-lookup"><span data-stu-id="8a09d-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)