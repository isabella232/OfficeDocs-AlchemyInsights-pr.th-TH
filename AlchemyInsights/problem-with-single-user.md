---
title: ปัญหากับผู้ใช้รายเดียว
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430209"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="f0b25-102">ปัญหากับผู้ใช้รายเดียว</span><span class="sxs-lookup"><span data-stu-id="f0b25-102">Problem with single user</span></span>

- <span data-ttu-id="f0b25-103">ผู้ใช้อาจยังไม่ได้เตรียมใช้งานเนื่องจากบริการยังไม่มีโอกาสที่จะประเมินผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f0b25-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="f0b25-104">ตรวจทานแนวทางสําหรับระยะเวลาการเตรียมใช้งานรวมถึงแถบความคืบหน้าบนหน้าการกําหนดค่าการเตรียมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f0b25-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="f0b25-105">ถ้าสถานะคงที่ที่ระบุไว้ในส่วนรายละเอียดเพิ่มเติมอยู่ก่อนวันที่ที่สร้าง/อัปเดต/ลบผู้ใช้ หมายความว่าเรายังไม่ได้ประเมินผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="f0b25-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="f0b25-106">ในสถานการณ์นี้ วิธีที่ดีที่สุดคือการรอให้บริการการเตรียมใช้งานเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="f0b25-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="f0b25-107">โปรดทราบว่าบริการของเราจะทราบถึงการเปลี่ยนแปลงของผู้ใช้ในระบบแหล่งข้อมูล (Cloud HR) เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f0b25-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="f0b25-108">ต้องมีการเปลี่ยนแปลงที่ถูกต้องในระบบแหล่งข้อมูลของ Azure AD เพื่อตรวจหาการเปลี่ยนแปลงและโฟลว์ลงใน Active Directory</span><span class="sxs-lookup"><span data-stu-id="f0b25-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="f0b25-109">บริการการเตรียมใช้งานประเมินผู้ใช้และกําหนดว่าไม่ควรเตรียมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="f0b25-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="f0b25-110">ถ้าคุณได้ตั้งค่าตัวกรองการซ้อนทับแอตทริบิวต์ โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ตรงตามเกณฑ์ที่คุณระบุ</span><span class="sxs-lookup"><span data-stu-id="f0b25-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="f0b25-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span><span class="sxs-lookup"><span data-stu-id="f0b25-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="f0b25-112">บริการการเตรียมใช้งานพยายามเตรียมใช้งานผู้ใช้ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="f0b25-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="f0b25-113">ดูสถานการณ์สมมติเหล่านี้ ตรวจทานแท็บการแก้ไขปัญหาและข้อแนะนะของบันทึกการเตรียมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="f0b25-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="f0b25-114">แอตทริบิวต์ที่ต้องมีกับผู้ใช้อาจหายไปใน Active Directory ภายในองค์กรหรือ Azure AD</span><span class="sxs-lookup"><span data-stu-id="f0b25-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f0b25-115">ตัวอย่างเช่น กฎการสร้าง userPrincipalName หรือ sAMAccountName ไม่ได้สร้างค่าที่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f0b25-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="f0b25-116">แอตทริบิวต์ที่ตรงกัน (โดยปกติจะเป็น employeeId) จะไม่แก้ไขให้ผู้ใช้ที่ไม่ซ้้ากันใน Active Directory ในองค์กรหรือ Azure AD</span><span class="sxs-lookup"><span data-stu-id="f0b25-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f0b25-117">ตัวอย่างเช่น มีผู้ใช้สองคนที่มีรหัสพนักงานเดียวกันใน AD และบริการส่งกลับรหัสข้อผิดพลาดจะระบุรายการเป้าหมายที่คัดลอกกันของรายการแหล่งข้อมูลเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="f0b25-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="f0b25-118">เมื่อต้องการรีวิวบันทึกของผู้ใช้และกลุ่มราย [เดียว ให้ดูตรวจทานบันทึกการเตรียมใช้งานเพื่อแก้ไขปัญหากับผู้ใช้](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)รายใดรายหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="f0b25-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
