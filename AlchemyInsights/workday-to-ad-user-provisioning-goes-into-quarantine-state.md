---
title: วันงานในการเตรียมใช้งานผู้ใช้ AD เข้าสู่สถานะการกักกัน
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482906"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="fe5ee-102">การเตรียมใช้งานผู้ใช้ของวันงานไปยัง AD เข้าสู่สถานะการกักกัน</span><span class="sxs-lookup"><span data-stu-id="fe5ee-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="fe5ee-103">**วันงานในการเตรียมใช้งานผู้ใช้ AD เข้าสู่สถานะการกักกัน และไม่มีการสร้างผู้ใช้ใน AD**</span><span class="sxs-lookup"><span data-stu-id="fe5ee-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="fe5ee-104">วันงานเป็นงานการเตรียมใช้งานผู้ใช้ AD ได้เข้าสู่สถานะการกักกัน และบันทึกการตรวจสอบแสดงเหตุการณ์ความล้มเหลวในการส่งออกด้วยข้อผิดพลาดข้อความแสดงข้อผิดพลาด **: OperationsError-SvcErr: มีข้อผิดพลาดการดําเนินการเกิดขึ้น ไม่มีการกําหนดค่าการอ้างอิงแบบเหนือชั้นของบริการไดเรกทอรี บริการไดเรกทอรีจึงไม่สามารถออกการอ้างอิงไปยังวัตถุที่อยู่ภายนอกฟอเรสต์** นี้</span><span class="sxs-lookup"><span data-stu-id="fe5ee-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="fe5ee-105">ข้อผิดพลาดนี้มักจะแสดงขึ้นถ้า Active Directory Container OU ไม่ได้ตั้งค่าอย่างถูกต้อง หรือมีปัญหากับการแมปนิพจน์ที่ใช้ **กับ parentDistinguishedName**</span><span class="sxs-lookup"><span data-stu-id="fe5ee-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="fe5ee-106">ตรวจสอบค่าเริ่มต้น OU **for New Users** parameter for typos</span><span class="sxs-lookup"><span data-stu-id="fe5ee-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="fe5ee-107">ตรวจสอบให้แน่ใจว่ามี OU ที่ระบุอยู่แล้วใน AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="fe5ee-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="fe5ee-108">ถ้าคุณใช้ **ParentDistinguishedName** ในการแมปแอตทริบิวต์ ตรวจสอบให้แน่ใจว่าค่านี้ประเมินเป็นคอนเทนเนอร์ที่รู้จักภายในโดเมน AD เสมอ</span><span class="sxs-lookup"><span data-stu-id="fe5ee-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="fe5ee-109">ตรวจสอบเหตุการณ์การส่งออกในบันทึกการตรวจสอบเพื่อดูค่าที่สร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="fe5ee-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="fe5ee-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="fe5ee-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

