---
title: การโยกย้ายจาก AIP ไปยัง MIP/Unified การติดป้ายในศูนย์การปฏิบัติตามนโยบาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674345"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="372aa-102">การโยกย้ายจาก AIP ไปยัง MIP/Unified การติดป้ายในศูนย์การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="372aa-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="372aa-103">เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP เพื่อรวมการติดป้ายในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายให้ทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="372aa-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="372aa-104">**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**</span><span class="sxs-lookup"><span data-stu-id="372aa-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="372aa-105">ถ้าคุณยังไม่ได้ทำให้เปิดหน้าต่างเบราว์เซอร์ใหม่และ[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="372aa-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="372aa-106">นำทางไปยังใบมีด**การป้องกันข้อมูลของ Azure**</span><span class="sxs-lookup"><span data-stu-id="372aa-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="372aa-107">ตัวอย่างเช่นบนเมนูฮับให้คลิก **บริการทั้งหมด** แล้วเริ่มพิมพ์ **ข้อมูล** ในกล่องตัวกรอง</span><span class="sxs-lookup"><span data-stu-id="372aa-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="372aa-108">เลือก**การป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="372aa-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="372aa-109">ถ้าคุณยังไม่ได้เข้าถึงใบมีดการป้องกันข้อมูลของ Azure ก่อนให้ดู [ขั้นตอนเพิ่มเติม](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) แบบครั้งเดียวเพื่อเพิ่มใบมีดนี้ไปยังพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="372aa-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="372aa-110">เมื่อต้องการเปิดใบมีดการป้องกันข้อมูลของ Azure คุณต้องมี [แผนพรีเมียมการป้องกันข้อมูลของ azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) หรือแผน Office ๓๖๕ที่มีการจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="372aa-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="372aa-111">ถ้าคุณมีหนึ่งในการสมัครใช้งานเหล่านี้แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้องให้ [ติดต่อฝ่ายสนับสนุนของไมโครซอฟท์](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) หรือใช้ช่องทางการสนับสนุนมาตรฐานของคุณ</span><span class="sxs-lookup"><span data-stu-id="372aa-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="372aa-112">ค้นหาตัวเลือก**จัดการ**เมนูแล้วเลือก**การเปิดใช้งานการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="372aa-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="372aa-113">คลิก **เปิดใช้งาน**แล้วยืนยันการดำเนินการของคุณ</span><span class="sxs-lookup"><span data-stu-id="372aa-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="372aa-114">เมื่อการเปิดใช้งานเสร็จสมบูรณ์แล้วแถบข้อมูลจะแสดงการ**เปิดใช้งานเสร็จเรียบร้อยแล้ว**</span><span class="sxs-lookup"><span data-stu-id="372aa-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="372aa-115">**โยกย้ายป้ายชื่อการป้องกันข้อมูล Azure ไปยังศูนย์การรักษาความปลอดภัยของ Office ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="372aa-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="372aa-116">ตรวจสอบให้แน่ใจว่าคุณได้เข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ระดับผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="372aa-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="372aa-117">นำทางไปยังใบมีด**การป้องกันข้อมูลของ Azure**</span><span class="sxs-lookup"><span data-stu-id="372aa-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="372aa-118">จากตัวเลือก**จัดการ**เมนูให้เลือกการ**ติดป้ายแบบครบวงจร**</span><span class="sxs-lookup"><span data-stu-id="372aa-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="372aa-119">บนหน้าการ **ป้องกันข้อมูลของ Azure-การติดป้ายชื่อแบบ** รวมให้คลิก **เปิดใช้งาน** แล้วทำตามคำแนะนำออนไลน์</span><span class="sxs-lookup"><span data-stu-id="372aa-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="372aa-120">**หมายเหตุ**: ตรวจสอบว่าคุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการโยกย้ายศูนย์การรักษาความปลอดภัย & การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="372aa-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="372aa-121">ดูบทความเหล่านี้สำหรับข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="372aa-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="372aa-122">คุณจำเป็นต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกำหนดค่าการป้องกันข้อมูลของ Azure หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบรายอื่นได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="372aa-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="372aa-123">ข้อมูลที่สำคัญเกี่ยวกับบทบาทการดูแลระบบหลังจากโยกย้ายไปยังศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="372aa-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="372aa-124">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ AIP เพื่อรวมการโยกย้ายการโยกย้ายไปยังศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายให้ดูที่การ[โยกย้ายป้ายชื่อ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="372aa-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
