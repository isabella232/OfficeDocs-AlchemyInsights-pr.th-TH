---
title: การเข้าถึงตามเงื่อนไขด้วย Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807678"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9a504-102">การเข้าถึงตามเงื่อนไขด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="9a504-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9a504-103">การใช้การ  **เข้าถึง**  แบบมีเงื่อนไขด้วย Intune จำเป็นต้องมี3ขั้นตอนดังนี้</span><span class="sxs-lookup"><span data-stu-id="9a504-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="9a504-104">สร้าง  **นโยบายการปฏิบัติตามนโยบาย**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) เพื่อกำหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าเป็นไปตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="9a504-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9a504-105">ตัวอย่างเช่นอุปกรณ์จำเป็นต้องมี pin อย่างน้อย6หลักก่อนที่จะถือว่าสอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="9a504-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="9a504-106">สร้าง **นโยบายการเข้าถึงตามเงื่อนไข**  ที่กำหนดว่าทรัพยากรใดบ้างที่ได้รับการป้องกันและต้องเป็นไปตามเงื่อนไขใดในการเข้าถึงแหล่งข้อมูลเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="9a504-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="9a504-107">ตัว[อย่างเช่น](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)อุปกรณ์ต้องสอดคล้องก่อนที่จะเข้าถึงอีเมลขององค์กร</span><span class="sxs-lookup"><span data-stu-id="9a504-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="9a504-108">ตรวจสอบให้แน่ใจ **ว่านโยบายการปฏิบัติตามกฎระเบียบ**  และ  **นโยบายการเข้าถึงตามเงื่อนไข**  จะถูกกำหนดเป้าหมายให้กับกลุ่มผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="9a504-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="9a504-109">การทำเช่นนี้อาจจำเป็นต้องสร้างกลุ่มผู้ใช้ที่เฉพาะเจาะจงใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9a504-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="9a504-110">**ลิงก์ที่มีประโยชน์:**</span><span class="sxs-lookup"><span data-stu-id="9a504-110">**Helpful links:**</span></span>

[<span data-ttu-id="9a504-111">ภาพรวมการปฏิบัติตามกฎระเบียบของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9a504-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9a504-112">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="9a504-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9a504-113">นโยบายการแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="9a504-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="9a504-114">เมื่อต้องการป้องกันอีเมล (Exchange online) จาก access โดยอุปกรณ์ noncompliant เอกสารทั้งสองต้องเป็นไปตาม:</span><span class="sxs-lookup"><span data-stu-id="9a504-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="9a504-115">ป้องกันการเข้าถึงอีเมลจากอุปกรณ์ที่ใช้ EAS</span><span class="sxs-lookup"><span data-stu-id="9a504-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="9a504-116">ป้องกันการเข้าถึงอีเมลจากอุปกรณ์ที่ใช้ไคลเอ็นต์การรับรองความถูกต้องที่ทันสมัยเช่น Outlook</span><span class="sxs-lookup"><span data-stu-id="9a504-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)