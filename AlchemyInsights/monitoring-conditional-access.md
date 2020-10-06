---
title: การตรวจสอบการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366447"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a3e74-102">การตรวจสอบการเข้าถึงแบบมีเงื่อนไขสำหรับ Exchange</span><span class="sxs-lookup"><span data-stu-id="a3e74-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a3e74-103">ผู้ใช้ที่กำหนดเป้าหมายด้วยการเข้าถึงแบบมีเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ตรงตามข้อกำหนดของการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="a3e74-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a3e74-104">เมื่อต้องการแก้ไขเราขอแนะนำวิธีแก้ไขปัญหาอย่างน้อยหนึ่งอย่างต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a3e74-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="a3e74-105">ถ้ามีการลงทะเบียนอุปกรณ์ให้ให้คำแนะนำให้ผู้ใช้ไปที่แอป Portal ของบริษัทและตรวจสอบว่าปรากฏในพอร์ทัลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="a3e74-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a3e74-106">ถ้าไม่ใช่ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a3e74-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="a3e74-107">ในพอร์ทัล Azure ให้ไปที่ Intune > การปฏิบัติตามข้อกำหนดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a3e74-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a3e74-108">ภายใต้การตรวจสอบให้คลิกการปฏิบัติตามข้อกำหนดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a3e74-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="a3e74-109">ดูรายงานการปฏิบัติตามนโยบายของอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้ได้รับการทำเครื่องหมายว่าสอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="a3e74-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="a3e74-110">ในพอร์ทัล Azure ให้ไปที่ Intune > การปฏิบัติตามข้อกำหนดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a3e74-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a3e74-111">ภายใต้จัดการให้คลิกนโยบาย</span><span class="sxs-lookup"><span data-stu-id="a3e74-111">Under Manage, click Policies.</span></span> <span data-ttu-id="a3e74-112">ในรายการนโยบายการปฏิบัติตามนโยบายให้ตรวจสอบว่าโปรไฟล์ถูกกำหนดให้กับอุปกรณ์ของผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a3e74-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a3e74-113">ถ้าไม่มีการกำหนดโปรไฟล์จากนั้น Intune จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="a3e74-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="a3e74-114">แก้ไขการกำหนดสิทธิ์การเข้าถึงตามเงื่อนไขของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a3e74-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="a3e74-115">ในพอร์ทัล Azure ให้ไปที่**Intune**  >  นโยบายการ**เข้าถึงแบบมีเงื่อนไข**  >  **Policies**ของ Intune</span><span class="sxs-lookup"><span data-stu-id="a3e74-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="a3e74-116">เลือกนโยบายจากรายการ</span><span class="sxs-lookup"><span data-stu-id="a3e74-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="a3e74-117">คลิกผู้ใช้และกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="a3e74-117">Click Users and groups.</span></span>
4. <span data-ttu-id="a3e74-118">เมื่อต้องการกำหนดเป้าหมายให้กับนโยบายบางอย่างที่มีใครบางคนให้เพิ่มลงในรายการรวม</span><span class="sxs-lookup"><span data-stu-id="a3e74-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="a3e74-119">เมื่อต้องการตรวจสอบให้แน่ใจว่าบุคคลถูกละเว้นจากนโยบายให้เพิ่มลงในรายการที่แยก</span><span class="sxs-lookup"><span data-stu-id="a3e74-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="a3e74-120">ลิงก์ที่มีประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="a3e74-120">Helpful links:</span></span>

[<span data-ttu-id="a3e74-121">ภาพรวมการปฏิบัติตามกฎระเบียบของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="a3e74-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a3e74-122">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="a3e74-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a3e74-123">นโยบายการแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="a3e74-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="a3e74-124">การตรวจสอบการปฏิบัติตามข้อกำหนดของอุปกรณ์ Intune</span><span class="sxs-lookup"><span data-stu-id="a3e74-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="a3e74-125">หมายเหตุ: ขั้นตอนเหล่านี้จะมีประโยชน์เฉพาะในการแก้ไขปัญหาการเข้าถึงแบบมีเงื่อนไขของ Azure Active Directory เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="a3e74-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="a3e74-126">นอกจากนี้ยังสามารถตรวจสอบความถูกต้องของอุปกรณ์ได้ด้วยการบล็อกการเข้าถึงอีเมลด้วยนโยบาย Exchange</span><span class="sxs-lookup"><span data-stu-id="a3e74-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="a3e74-127">คุณสามารถดูข้อมูลเพิ่มเติมเกี่ยวกับการจัดการอุปกรณ์ Exchange ได้[ที่นี่](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)</span><span class="sxs-lookup"><span data-stu-id="a3e74-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
