---
title: การย้ายข้อมูลจาก AIP ไปยังการติดป้ายชื่อ MIP/รวมในศูนย์การปฏิบัติตามกฎระเบียบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236566"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="98716-102">การย้ายข้อมูลจาก AIP ไปยังการติดป้ายชื่อ MIP/รวมในศูนย์การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="98716-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="98716-103">เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP ไปยัง Unified Labeling ในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="98716-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="98716-104">**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**</span><span class="sxs-lookup"><span data-stu-id="98716-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="98716-105">ถ้าคุณยังไม่ได้ทํา ให้เปิดหน้าต่างเบราว์เซอร์ใหม่แล้ว[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="98716-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="98716-106">นําทางไปยังใบ**ป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="98716-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="98716-107">ตัวอย่างเช่น บนเมนูฮับ คลิก**บริการทั้งหมด**และเริ่มพิมพ์**ข้อมูล**ในกล่องตัวกรอง</span><span class="sxs-lookup"><span data-stu-id="98716-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="98716-108">เลือก**การป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="98716-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="98716-109">ถ้าคุณยังไม่ได้เข้าถึงใบป้องกันข้อมูล Azure ก่อน ดู[ขั้นตอนเพิ่มเติม](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)แบบครั้งเดียวเพื่อเพิ่มใบนี้ไปยังพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="98716-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="98716-110">เมื่อต้องการเปิดใบป้องกันข้อมูล Azure คุณต้องมี[แผน Azure ป้องกันข้อมูลแบบพิเศษ](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)หรือแผน Office 365 ที่มีการจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="98716-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="98716-111">ถ้าคุณมีการสมัครใช้งานเหล่านี้แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้อง[โปรดติดต่อฝ่ายสนับสนุนของ Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)หรือใช้ช่องทางการสนับสนุนมาตรฐานของคุณ</span><span class="sxs-lookup"><span data-stu-id="98716-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="98716-112">ค้นหาตัวเลือก**เมนูจัดการ**และเลือก**การเปิดใช้งานการป้องกัน**</span><span class="sxs-lookup"><span data-stu-id="98716-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="98716-113">คลิก**เปิดใช้งาน**แล้วยืนยันการดําเนินการของคุณ</span><span class="sxs-lookup"><span data-stu-id="98716-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="98716-114">เมื่อเปิดใช้งานเสร็จสมบูรณ์**Activation finished successfully**</span><span class="sxs-lookup"><span data-stu-id="98716-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="98716-115">**โยกย้ายป้ายชื่อการป้องกันข้อมูล Azure ไปยังศูนย์การปฏิบัติตามข้อกําหนด&ความปลอดภัยของ Office 365**</span><span class="sxs-lookup"><span data-stu-id="98716-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="98716-116">ตรวจสอบให้แน่ใจว่า คุณได้เข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ของผู้ดูแลระบบส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="98716-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="98716-117">นําทางไปยังใบ**ป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="98716-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="98716-118">จากตัวเลือก**จัดการ**เมนู ให้เลือก**การติดป้ายชื่อแบบรวม**</span><span class="sxs-lookup"><span data-stu-id="98716-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="98716-119">บน**การป้องกันข้อมูล Azure - ใบติดฉลากแบบรวม**คลิก**เปิดใช้งาน**และทําตามคําแนะนําแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="98716-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="98716-120">**หมายเหตุ**: ตรวจสอบว่า คุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการรักษาความปลอดภัย&ศูนย์ปฏิบัติตามกฎระเบียบการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="98716-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="98716-121">ดูบทความเหล่านี้สําหรับข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="98716-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="98716-122">คุณต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกําหนดค่าการป้องกันข้อมูล Azure หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบอื่นได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="98716-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="98716-123">ข้อมูลสําคัญเกี่ยวกับบทบาทการดูแลระบบหลังจากโยกย้ายไปยังศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="98716-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="98716-124">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับ AIP ไปยังการโยกย้ายการติดฉลากแบบรวมไปยังความปลอดภัยและศูนย์การปฏิบัติตามกฎระเบียบ ให้ดูที่[โยกย้ายป้ายชื่อ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="98716-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
