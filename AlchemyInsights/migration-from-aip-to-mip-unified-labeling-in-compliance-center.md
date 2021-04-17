---
title: การโยกย้ายจาก AIP ไปยังป้ายชื่อ MIP/Unified ในศูนย์การปฏิบัติตามข้อบังคับ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825390"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="1e8a0-102">การโยกย้ายจาก AIP ไปยังป้ายชื่อ MIP/Unified ในศูนย์การปฏิบัติตามข้อบังคับ</span><span class="sxs-lookup"><span data-stu-id="1e8a0-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="1e8a0-103">เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP ไปยังป้ายชื่อแบบครบวงจรในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย ให้ปฏิบัติดังนี้</span><span class="sxs-lookup"><span data-stu-id="1e8a0-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="1e8a0-104">**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="1e8a0-105">ถ้าคุณยังไม่ได้เปิด ให้เปิดหน้าต่างเบราว์เซอร์ใหม่และ[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="1e8a0-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="1e8a0-106">นําทางไปยัง **เบลด Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="1e8a0-107">ตัวอย่างเช่น บนเมนูฮับ ให้คลิก **บริการทั้งหมด** แล้วเริ่ม **พิมพ์** ข้อมูล ในกล่อง ตัวกรอง</span><span class="sxs-lookup"><span data-stu-id="1e8a0-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="1e8a0-108">เลือก **Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="1e8a0-109">ถ้าคุณไม่เคยเข้าถึงเบลด Azure Information Protection มาก่อน ให้ดูขั้นตอนเพิ่มเติมแบบใช้ [เวลา](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) เดียวเพื่อเพิ่มเบลดนี้ลงในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="1e8a0-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="1e8a0-110">เมื่อต้องการเปิดเบลด Azure Information Protection คุณต้องมีแผน [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) หรือแผน Office 365 ที่มีการจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="1e8a0-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="1e8a0-111">ถ้าคุณมีหนึ่งในการสมัครใช้งานเหล่านี้ แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้อง ติดต่อฝ่ายสนับสนุนของ [Microsoft หรือใช้](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) แชนเนลการสนับสนุนมาตรฐานของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e8a0-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="1e8a0-112">ค้นหา **ตัวเลือก** เมนู จัดการ แล้วเลือก **การเปิดใช้งาน** การป้องกัน</span><span class="sxs-lookup"><span data-stu-id="1e8a0-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="1e8a0-113">คลิก **เปิดใช้งาน** แล้วยืนยันการทํางานของคุณ</span><span class="sxs-lookup"><span data-stu-id="1e8a0-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="1e8a0-114">เมื่อเปิดใช้งานเสร็จสมบูรณ์ แถบข้อมูลจะแสดง การเปิดใช้งาน **เสร็จสมบูรณ์**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="1e8a0-115">**โยกย้ายป้ายชื่อ Azure Information Protection ไปยังศูนย์การรักษา& Office 365**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="1e8a0-116">ตรวจสอบให้แน่ใจว่าคุณเข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="1e8a0-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="1e8a0-117">นําทางไปยัง **เบลด Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="1e8a0-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="1e8a0-118">จาก **ตัวเลือก** เมนูจัดการ **ให้เลือก การติดป้ายผนึก** แบบรวม</span><span class="sxs-lookup"><span data-stu-id="1e8a0-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="1e8a0-119">บน **Azure Information Protection - ใบป้ายชื่อแบบรวม** ให้คลิก **เปิดใช้งาน และ** ปฏิบัติตามคําแนะนําแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="1e8a0-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="1e8a0-120">**หมายเหตุ**: ตรวจสอบว่าคุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการโยกย้ายศูนย์&การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="1e8a0-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="1e8a0-121">ดูบทความเหล่านี้เพื่อดูข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="1e8a0-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="1e8a0-122">คุณต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกําหนดค่า Azure Information Protection หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบคนอื่นได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1e8a0-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="1e8a0-123">ข้อมูลสําคัญเกี่ยวกับบทบาทผู้ดูแลระบบหลังจากการโยกย้ายไปยังศูนย์&การปฏิบัติตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="1e8a0-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="1e8a0-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="1e8a0-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
