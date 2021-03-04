---
title: ตรวจสอบการเข้าถึงตามเงื่อนไขของ Intuns
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428309"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="9b14f-102">ตรวจสอบการเข้าถึงตามเงื่อนไขของ Intuns</span><span class="sxs-lookup"><span data-stu-id="9b14f-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="9b14f-103">ผู้ใช้ที่เป็นเป้าหมายของการเข้าถึงตามเงื่อนไขจะได้รับอีเมลแจ้งเตือนถ้าพวกเขาไม่ตรงตามข้อกฎหมายการเข้าถึงขององค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="9b14f-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9b14f-104">เมื่อต้องการแก้ไขปัญหา เราขอแนะนนะให้แก้ไขปัญหาอย่างน้อยหนึ่งวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9b14f-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="9b14f-105">ถ้าอุปกรณ์ได้รับการลงทะเบียนแล้ว ให้แนะนาให้ผู้ใช้ไปที่แอป Company Portal และตรวจสอบว่าอุปกรณ์ปรากฏในพอร์ทัลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="9b14f-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9b14f-106">ถ้าไม่ ผู้ใช้ต้องลงทะเบียนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9b14f-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="9b14f-107">ในพอร์ทัล Azure ให้ไปที่ **การปฏิบัติตามนโยบายอุปกรณ์ Intuned**  >  </span><span class="sxs-lookup"><span data-stu-id="9b14f-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="9b14f-108">เมื่อต้องการดูรายงานการปฏิบัติตามนโยบายอุปกรณ์ของคุณเพื่อตรวจสอบว่าอุปกรณ์ของผู้ใช้ถูกระบุว่าปฏิบัติตามนโยบายแล้ว ภายใต้ **จอภาพ** ให้คลิก **การปฏิบัติตามนโยบาย** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9b14f-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="9b14f-109">ในพอร์ทัล Azure ให้ไปที่ **การปฏิบัติตามนโยบายอุปกรณ์ Intuned**  >  </span><span class="sxs-lookup"><span data-stu-id="9b14f-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="9b14f-110">ภายใต้ **จัดการ\*\*\*\*ให้คลิก** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="9b14f-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="9b14f-111">ในรายการนโยบายการปฏิบัติตามนโยบาย ให้ตรวจสอบว่าโปรไฟล์ถูกมอบหมายให้กับอุปกรณ์ของผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="9b14f-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9b14f-112">ถ้าไม่มีการมอบหมายโปรไฟล์ Intun1 จะไม่สามารถยืนยันสถานะการปฏิบัติตามนโยบายของอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="9b14f-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="9b14f-113">แก้ไขการมอบหมายการเข้าถึงตามเงื่อนไขของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="9b14f-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="9b14f-114">ในพอร์ทัล Azure ให้นํา **ทางไปยังนโยบายการเข้าถึงตามเงื่อนไข Intuned**  >    >  เลือกนโยบายจากรายการ **แล้วคลิกผู้ใช้และ** กลุ่ม</span><span class="sxs-lookup"><span data-stu-id="9b14f-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="9b14f-115">เมื่อต้องการตั้งเป้าหมายนโยบายใดนโยบายหนึ่งให้กับบางคน ให้เพิ่มพวกเขา **ลงในรายการ** รวม</span><span class="sxs-lookup"><span data-stu-id="9b14f-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="9b14f-116">เพื่อให้แน่ใจว่าได้ละเว้นบุคคลใดบุคคลหนึ่งจากนโยบาย ให้เพิ่มบุคคลนั้น **ลงในรายการ** ยกเว้น</span><span class="sxs-lookup"><span data-stu-id="9b14f-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="9b14f-117">**ลิงก์ที่เป็นประโยชน์:**</span><span class="sxs-lookup"><span data-stu-id="9b14f-117">**Helpful links:**</span></span>

- [<span data-ttu-id="9b14f-118">ภาพรวมการปฏิบัติตามนโยบายอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="9b14f-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="9b14f-119">การแก้ไขปัญหา CA</span><span class="sxs-lookup"><span data-stu-id="9b14f-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="9b14f-120">การแก้ไขปัญหานโยบาย</span><span class="sxs-lookup"><span data-stu-id="9b14f-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="9b14f-121">การตรวจสอบการปฏิบัติตามนโยบายอุปกรณ์ Intun1</span><span class="sxs-lookup"><span data-stu-id="9b14f-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="9b14f-122">ขั้นตอนเหล่านี้มีประโยชน์ในการแก้ไขปัญหาการเข้าถึงตามเงื่อนไขของฟีเจอร์ Azure Active Directory เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="9b14f-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="9b14f-123">นอกจากนี้ยังสามารถกักกันอุปกรณ์ที่บล็อกการเข้าถึงอีเมลด้วยนโยบาย Exchange</span><span class="sxs-lookup"><span data-stu-id="9b14f-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="9b14f-124">ข้อมูลเพิ่มเติมเกี่ยวกับการจัดการอุปกรณ์ Exchange [**สามารถพบได้ที่นี่**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="9b14f-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
