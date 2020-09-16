---
title: ป้ายชื่อความลับไม่ปรากฏขึ้น
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801203"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="7a1da-102">ป้ายชื่อความลับไม่ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="7a1da-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="7a1da-103">ป้ายความลับจะช่วยให้คุณสามารถจัดประเภทและช่วยป้องกันเนื้อหาที่มีความสำคัญของคุณได้</span><span class="sxs-lookup"><span data-stu-id="7a1da-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="7a1da-104">พวกเขาสามารถสร้างขึ้นได้ในศูนย์การปฏิบัติตามนโยบายของ Microsoft ๓๖๕, ศูนย์การรักษาความปลอดภัยของ microsoft ๓๖๕หรือ Microsoft ๓๖๕ความปลอดภัย & ศูนย์การปฏิบัติตามนโยบายภายใต้การจัดประเภท > ป้ายชื่อความลับ</span><span class="sxs-lookup"><span data-stu-id="7a1da-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="7a1da-105">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับฟีเจอร์นี้ให้ดู[ที่ภาพรวมของป้ายชื่อความลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="7a1da-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="7a1da-106">ถ้าคุณกำหนดค่าป้ายชื่อความลับของคุณแต่ไม่ปรากฏในแอป Microsoft ๓๖๕ให้ตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7a1da-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="7a1da-107">ยืนยันว่ามีการ [เผยแพร่](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) ป้ายความลับของผู้ใช้และกลุ่มที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="7a1da-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="7a1da-108">ยืนยันว่าผู้ใช้กำลังใช้แอปที่สนับสนุนป้ายชื่อความลับ-ดู[ป้ายชื่อความลับในเอกสารของคุณ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)</span><span class="sxs-lookup"><span data-stu-id="7a1da-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="7a1da-109">ถ้าคุณกำลัง[โยกย้ายป้ายชื่อการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)โปรดทราบข้อควรพิจารณาที่แสดงรายการไว้[ที่นี่](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)</span><span class="sxs-lookup"><span data-stu-id="7a1da-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="7a1da-110">การสนับสนุนการป้องกันการสูญหายของข้อมูล (DLP): ในขณะนี้มีเฉพาะป้ายการเก็บข้อมูลเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP ได้</span><span class="sxs-lookup"><span data-stu-id="7a1da-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="7a1da-111">การสนับสนุนสำหรับป้ายชื่อความลับในนโยบาย DLP ยังไม่พร้อมใช้งานแต่เรากำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="7a1da-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="7a1da-112">เมื่อมีการเปิดใช้งานการเข้ารหัสลับบนป้ายชื่อความลับคุณสามารถเลือกได้ว่าจะ:</span><span class="sxs-lookup"><span data-stu-id="7a1da-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="7a1da-113">กำหนดสิทธิ์เดี๋ยวนี้</span><span class="sxs-lookup"><span data-stu-id="7a1da-113">Assign permissions now</span></span>
    - <span data-ttu-id="7a1da-114">อนุญาตให้ผู้ใช้กำหนดสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="7a1da-114">Let users assign permissions</span></span>


<span data-ttu-id="7a1da-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาที่เป็นไปได้ให้ดู[ที่ปัญหาที่ทราบเกี่ยวกับป้ายชื่อความลับ](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)</span><span class="sxs-lookup"><span data-stu-id="7a1da-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>