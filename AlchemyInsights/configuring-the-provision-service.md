---
title: การกําหนดค่าบริการเตรียมใช้งาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484046"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="adf27-102">การกําหนดค่าบริการเตรียมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="adf27-102">Configuring the Provision service</span></span>

<span data-ttu-id="adf27-103">เพื่อให้การเตรียมใช้งานผู้ใช้โดยอัตโนมัติใช้งานได้ Azure AD ต้องการข้อมูลรับรองที่ถูกต้องที่อนุญาตให้เชื่อมต่อกับ API ของบริการเว็บของ Workday</span><span class="sxs-lookup"><span data-stu-id="adf27-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="adf27-104">นอกจากนี้ ปุ่มทดสอบการเชื่อมต่อบนวันการเตรียมใช้งานผู้ใช้ AD ยังตรวจสอบความถูกต้องถ้าสามารถเชื่อมต่อกับ Azure AD Connect Provisioning Agent ที่เชื่อมโยงกับโดเมน AD</span><span class="sxs-lookup"><span data-stu-id="adf27-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="adf27-105">ถ้าพอร์ทัล Azure ส่งกลับข้อผิดพลาดเมื่อบันทึกข้อมูลอ้างอิง ให้ปฏิบัติตามขั้นตอนที่แนะนาทางด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="adf27-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="adf27-106">ยืนยันว่าคุณได้กําหนดค่าบัญชีผู้ใช้ระบบการรวมของวันงานตามที่ระบุไว้ในส่วนบทช่วยสอน กําหนดค่า[ผู้ใช้ระบบการรวมใน Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="adf27-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="adf27-107">ยืนยันว่า Azure AD Connect Provisioning Agent Service เปิดใช้งานอยู่และใช้งานบนเซิร์ฟเวอร์ Windows ภายในองค์กรของคุณโดยใช้คอนโซลการจัดการบริการ</span><span class="sxs-lookup"><span data-stu-id="adf27-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="adf27-108">คุณยังสามารถตรวจสอบสถานะของตัวแทนในพอร์ทัล Azure โดยการคลิกปุ่มดูตัวแทนภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="adf27-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="adf27-109">ตรวจสอบให้แน่ใจว่าคุณใส่ค่าเขตข้อมูล "ชื่อผู้ใช้งาน" โดยใช้รูปแบบusername@workday-ผู้เช่า</span><span class="sxs-lookup"><span data-stu-id="adf27-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="adf27-110">ถ้าชื่อผู้เช่าวันงานหายไป การรับรองความถูกต้องวันงานล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="adf27-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="adf27-111">ถ้าคุณกําหนดค่าการรวมกับผู้เช่าการใช้งานวันงาน ให้สังเกตชั่วโมงการหยุดใช้งานที่กําหนดไว้ของผู้เช่าวันงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="adf27-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="adf27-112">วันงานได้จัดเวลาหยุดให้บริการผู้เช่าในช่วงวันหยุดสุดสัปดาห์ (โดยปกติคือช่วงเย็นวันศุกร์ถึงเช้าวันเสาร์) และความล้มเหลวในการเชื่อมต่อระหว่างหน้าต่างการหยุดให้บริการนี้เป็นปัญหาที่ทราบแล้วซึ่งแก้ไขโดยอัตโนมัติทันทีที่ผู้เช่าการปรับใช้กลับมาออนไลน์</span><span class="sxs-lookup"><span data-stu-id="adf27-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="adf27-113">ในบางกรณี คุณอาจเห็นข้อผิดพลาดนี้ถ้ารหัสผ่านของผู้ใช้ Integration System เปลี่ยนแปลงไปเนื่องจากการรีเฟรชผู้เช่า หรือถ้าบัญชีอยู่ในสถานะถูกล็อกหรือหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="adf27-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="adf27-114">โปรดตรวจสอบสถานะของผู้ใช้ระบบการรวมกับผู้ดูแลระบบของวันการงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="adf27-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="adf27-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="adf27-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
