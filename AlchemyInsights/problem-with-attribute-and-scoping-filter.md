---
title: ปัญหาเกี่ยวกับแอตทริบิวต์และตัวกรองการโควตา
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482924"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="31c9a-102">ปัญหาเกี่ยวกับแอตทริบิวต์และตัวกรองการโควตา</span><span class="sxs-lookup"><span data-stu-id="31c9a-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="31c9a-103">**ปัญหากับค่า UPN ที่ขัดแย้งกัน**</span><span class="sxs-lookup"><span data-stu-id="31c9a-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="31c9a-104">วันการเตรียมใช้งานผู้ใช้ AD ไปยังการเตรียมใช้งานผู้ใช้ AD จะแสดงข้อความแสดงข้อผิดพลาด **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**</span><span class="sxs-lookup"><span data-stu-id="31c9a-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="31c9a-105">การดําเนินการล้มเหลวเนื่องจากค่า UPN ที่ให้ไว้เพื่อการเพิ่ม/การปรับเปลี่ยนไม่ครอบคลุมฟอเรสต์ที่ไม่ซ้ได้</span><span class="sxs-lookup"><span data-stu-id="31c9a-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="31c9a-106">รายละเอียดข้อผิดพลาด: **CONSTRAINT_ATT_TYPE - userPrincipalName**</span><span class="sxs-lookup"><span data-stu-id="31c9a-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="31c9a-107">ค่า **userPrincipalName** ที่ตัวเชื่อมต่อ Workday พยายามตั้งค่าเมื่อสร้างบัญชีผู้ใช้ AD มีอยู่แล้วในโดเมน AD เป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="31c9a-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="31c9a-108">ซึ่งแสดงว่ามีผู้ใช้ (1) รายอยู่แล้ว และการตรวจสอบ ID ที่ตรงกันล้มเหลวของผู้ใช้หรือ (2) กฎการสร้าง UPN สร้างค่าที่ขัดแย้งกัน</span><span class="sxs-lookup"><span data-stu-id="31c9a-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="31c9a-109">ต่อไปนี้คือขั้นตอนการแก้ปัญหาที่แนะนา:</span><span class="sxs-lookup"><span data-stu-id="31c9a-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="31c9a-110">ถ้าผู้ใช้มีอยู่แล้ว และการตรวจสอบ ID ที่ตรงกันไม่สามารถลิงก์บัญชี Workday กับบัญชี Active Directory ได้ ให้ตรวจสอบว่าแอตทริบิวต์ ID ที่ตรงกันหรือไม่ (โดยทั่วไปคือ **employeeID)** ในทั้งวันงานและ AD ตรงกันทุกอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="31c9a-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="31c9a-111">ถ้าข้อมูลไม่ตรงกัน อาจเป็นปัญหาข้อมูลที่ต้องได้รับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="31c9a-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="31c9a-112">ตัวอย่างเช่น ถ้า EmployeeID ใน Workday คือ 001052 และใน AD คือ 1052 กลไกจัดการการเตรียมใช้งานจะไม่สามารถลิงก์สองบัญชีและจะพยายามสร้างผู้ใช้ที่มีอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="31c9a-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="31c9a-113">โซลูชันในกรณีนี้คือการเปลี่ยนค่า **EmployeeID** ใน AD ให้รวมเลขศูนย์ที่ส่วนหน้าเพื่อใส่เป็น 001052</span><span class="sxs-lookup"><span data-stu-id="31c9a-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="31c9a-114">ถ้านิพจน์ที่สร้างโดย UPN ไม่ได้สร้างค่าที่ไม่ซ้>า ให้พิจารณาใช้ฟังก์ชัน de-duplication **SelectUniqueValus** เพื่อสร้างค่าที่ไม่ซ้>ในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="31c9a-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="31c9a-115">**วันของงานในการเตรียมใช้งานผู้ใช้ AD ไม่ได้ตั้งค่าแอตทริบิวต์ของผู้จัดการให้กับบัญชีผู้ใช้ AD**</span><span class="sxs-lookup"><span data-stu-id="31c9a-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="31c9a-116">งานวันงานเป็นงานการเตรียมใช้งานผู้ใช้ AD **ไม่ได้ตั้งค่า** แอตทริบิวต์ผู้จัดการให้กับบัญชีผู้ใช้ AD</span><span class="sxs-lookup"><span data-stu-id="31c9a-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="31c9a-117">มีสถานการณ์ที่เป็นไปได้สองสถานการณ์เมื่อพบลักษณะการนี้:</span><span class="sxs-lookup"><span data-stu-id="31c9a-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="31c9a-118">ผู้จัดการในวันงานไม่สามารถแก้ไขเป็นบัญชีผู้ใช้ AD ที่สอดคล้องกันได้ เนื่องจากผู้จัดการไม่อยู่ในขอบเขต</span><span class="sxs-lookup"><span data-stu-id="31c9a-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="31c9a-119">ในสถานการณ์ **โดเมน AD หลาย** โดเมน ผู้จัดการในวันงานจะไม่แสดงในโดเมนเดียวกันกับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="31c9a-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="31c9a-120">ลองขั้นตอนเหล่านี้เพื่อแก้ไขปัญหา:</span><span class="sxs-lookup"><span data-stu-id="31c9a-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="31c9a-121">ถ้าคุณได้กําหนดตัวกรองการกําหนดขอบเขตไว้ ก่อนอื่นให้ตรวจสอบถ้าผู้จัดการอยู่ในขอบเขตและเป็นไปตามส่วนสั่งการกําหนดขอบเขต</span><span class="sxs-lookup"><span data-stu-id="31c9a-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="31c9a-122">ถ้าผู้จัดการไม่เป็นไปตามตัวกรองการหาขอบเขต ให้เปลี่ยนตัวกรองเพื่อให้ผู้จัดการอยู่ในขอบเขตของการดําเนินการเตรียมใช้งานด้วย</span><span class="sxs-lookup"><span data-stu-id="31c9a-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="31c9a-123">ถ้าคุณมีโดเมน AD หลายโดเมน ตัวเชื่อมต่อจะมีข้อจํากัดที่ทราบแล้วว่าไม่สามารถแก้ไขการอ้างอิงตัวจัดการข้ามโดเมนได้</span><span class="sxs-lookup"><span data-stu-id="31c9a-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="31c9a-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="31c9a-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













