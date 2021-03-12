---
title: การตรวจสอบการเข้าถึงตามเงื่อนไข
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708693"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="91034-102">การตรวจสอบการเข้าถึงตามเงื่อนไขใน Exchange</span><span class="sxs-lookup"><span data-stu-id="91034-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="91034-103">ผู้ใช้ที่เป็นเป้าหมายของการเข้าถึงตามเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ตรงตามข้อกฎหมายการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="91034-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="91034-104">เมื่อต้องการแก้ไขปัญหา เราขอแนะนนะให้แก้ไขปัญหาอย่างน้อยหนึ่งวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="91034-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="91034-105">ถ้าอุปกรณ์ได้รับการลงทะเบียนแล้ว ให้แนะนาให้ผู้ใช้ไปที่แอป Company Portal และตรวจสอบว่าอุปกรณ์ปรากฏในพอร์ทัลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="91034-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="91034-106">ถ้าไม่ ผู้ใช้ควรลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="91034-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="91034-107">ในพอร์ทัล Azure ให้ไปที่ Intuned >ปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="91034-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="91034-108">ภายใต้ ตรวจสอบ ให้คลิก การปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="91034-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="91034-109">ดูรายงานการปฏิบัติตามนโยบายของอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้มีเครื่องหมายเป็นปฏิบัติตามนโยบายแล้ว</span><span class="sxs-lookup"><span data-stu-id="91034-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="91034-110">ในพอร์ทัล Azure ให้ไปที่ Intuned >ปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="91034-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="91034-111">ภายใต้ จัดการ ให้คลิก นโยบาย</span><span class="sxs-lookup"><span data-stu-id="91034-111">Under Manage, click Policies.</span></span> <span data-ttu-id="91034-112">ในรายการนโยบายการปฏิบัติตามนโยบาย ให้ตรวจสอบว่าโปรไฟล์ถูกมอบหมายให้กับอุปกรณ์ของผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="91034-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="91034-113">ถ้าไม่มีการมอบหมายโปรไฟล์ Intun1 จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="91034-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="91034-114">แก้ไขการมอบหมายการเข้าถึงตามเงื่อนไขของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="91034-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="91034-115">ในพอร์ทัล Azure ให้ไปที่ **นโยบายการเข้าถึงตามเงื่อนไขของ Intuned**  >    >  </span><span class="sxs-lookup"><span data-stu-id="91034-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="91034-116">เลือกนโยบายจากรายการ</span><span class="sxs-lookup"><span data-stu-id="91034-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="91034-117">คลิก ผู้ใช้และกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="91034-117">Click Users and groups.</span></span>
4. <span data-ttu-id="91034-118">เมื่อต้องการตั้งเป้าหมายนโยบายใดนโยบายหนึ่งให้กับบางคน ให้เพิ่มพวกเขาลงในรายการ รวม</span><span class="sxs-lookup"><span data-stu-id="91034-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="91034-119">เพื่อให้แน่ใจว่าได้ละเว้นบุคคลใดบุคคลหนึ่งจากนโยบาย ให้เพิ่มบุคคลนั้นลงในรายการ ยกเว้น</span><span class="sxs-lookup"><span data-stu-id="91034-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="91034-120">ลิงก์ที่เป็นประโยชน์:</span><span class="sxs-lookup"><span data-stu-id="91034-120">Helpful links:</span></span>

[<span data-ttu-id="91034-121">ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="91034-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="91034-122">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="91034-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="91034-123">การแก้ไขปัญหานโยบาย</span><span class="sxs-lookup"><span data-stu-id="91034-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="91034-124">การตรวจสอบการปฏิบัติตามนโยบายอุปกรณ์ Intun1</span><span class="sxs-lookup"><span data-stu-id="91034-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="91034-125">หมายเหตุ: ขั้นตอนเหล่านี้มีประโยชน์ในการแก้ไขปัญหาการเข้าถึงตามเงื่อนไขของฟีเจอร์ Azure Active Directory เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="91034-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="91034-126">นอกจากนี้ยังสามารถกักกันอุปกรณ์ที่บล็อกการเข้าถึงอีเมลด้วยนโยบาย Exchange</span><span class="sxs-lookup"><span data-stu-id="91034-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="91034-127">ข้อมูลเพิ่มเติมเกี่ยวกับการจัดการอุปกรณ์ Exchange สามารถพบได้ [ที่นี่ https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) ](</span><span class="sxs-lookup"><span data-stu-id="91034-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
