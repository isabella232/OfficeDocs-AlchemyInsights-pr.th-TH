---
title: ป้ายชื่อความไวไม่ปรากฏ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581034"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="7d495-102">ป้ายชื่อความไวไม่ปรากฏ</span><span class="sxs-lookup"><span data-stu-id="7d495-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="7d495-103">ป้ายความไวช่วยให้คุณสามารถจัดประเภทและช่วยปกป้องเนื้อหาที่ละเอียดอ่อนของคุณ</span><span class="sxs-lookup"><span data-stu-id="7d495-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="7d495-104">พวกเขาสามารถสร้างขึ้นในศูนย์การปฏิบัติตามกฎระเบียบ Microsoft 365 ศูนย์รักษาความปลอดภัย Microsoft 365 หรือความปลอดภัยของ Microsoft 365 &ศูนย์การปฏิบัติตามกฎระเบียบภายใต้ป้ายชื่อ>ความอ่อนไหวของการจําแนก</span><span class="sxs-lookup"><span data-stu-id="7d495-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="7d495-105">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับคุณลักษณะนี้ ให้ดูที่[ภาพรวมของป้ายชื่อความไว](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="7d495-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="7d495-106">ถ้าคุณกําหนดค่าป้ายชื่อความไวของคุณ แต่ป้ายชื่อเหล่านั้นไม่ปรากฏในแอป Microsoft 365 ให้ตรวจสอบสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7d495-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="7d495-107">ยืนยันว่าได้มีการ[ประกาศ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do)ป้ายชื่อความไวต่อผู้ใช้และกลุ่มที่คุณต้องการแล้ว</span><span class="sxs-lookup"><span data-stu-id="7d495-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="7d495-108">ยืนยันว่าผู้ใช้ใช้แอปที่รองรับป้ายกํากับความไว - ดู[ป้ายความไวในเอกสารของคุณ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)</span><span class="sxs-lookup"><span data-stu-id="7d495-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="7d495-109">ถ้าคุณกําลัง[here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)[ย้ายข้อมูลป้าย Azure ป้องกัน](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="7d495-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="7d495-110">การสนับสนุนการป้องกันข้อมูลสูญหาย (DLP): ปัจจุบันเฉพาะป้ายกํากับการเก็บรักษาเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="7d495-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="7d495-111">การสนับสนุนสําหรับป้ายความไวในนโยบาย DLP จะไม่พร้อมใช้งาน แต่เรากําลังดําเนินการอยู่</span><span class="sxs-lookup"><span data-stu-id="7d495-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="7d495-112">เมื่อเปิดใช้งานการเข้ารหัสบนป้ายชื่อความไว คุณสามารถเลือกอย่างใดอย่างหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7d495-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="7d495-113">กําหนดสิทธิ์เดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="7d495-113">Assign permissions now</span></span>
    - <span data-ttu-id="7d495-114">อนุญาตให้ผู้ใช้กําหนดสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="7d495-114">Let users assign permissions</span></span>


<span data-ttu-id="7d495-115">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาที่เป็นไปได้ ให้ดูที่[ปัญหาที่ทราบเกี่ยวกับป้ายความไว](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)</span><span class="sxs-lookup"><span data-stu-id="7d495-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>