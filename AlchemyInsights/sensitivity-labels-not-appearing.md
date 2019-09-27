---
title: ไม่ปรากฏป้ายชื่อความไว
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207244"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="1cd2f-102">ไม่ปรากฏป้ายชื่อความไว</span><span class="sxs-lookup"><span data-stu-id="1cd2f-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="1cd2f-103">ป้ายความไวช่วยให้คุณสามารถจัดประเภทและช่วยปกป้องเนื้อหาที่ละเอียดอ่อนของคุณ</span><span class="sxs-lookup"><span data-stu-id="1cd2f-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="1cd2f-104">พวกเขาสามารถสร้างขึ้นในศูนย์การปฏิบัติตามกฎระเบียบของ Microsoft ๓๖๕ศูนย์รักษาความปลอดภัย Microsoft ๓๖๕หรือสำนักงาน๓๖๕ความปลอดภัย & การปฏิบัติตามกฎระเบียบภายใต้การจัดประเภท > ป้ายความไว</span><span class="sxs-lookup"><span data-stu-id="1cd2f-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="1cd2f-105">หากต้องการเรียนรู้เพิ่มเติมเกี่ยวกับคุณลักษณะนี้โปรดดูที่[ภาพรวมของป้ายความไว](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="1cd2f-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="1cd2f-106">หากคุณกำหนดค่าป้ายความไวของคุณแต่จะไม่ปรากฏในแอป Office ให้ตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1cd2f-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="1cd2f-107">ยืนยันว่าป้ายความไวได้รับการ[เผยแพร่](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)ไปยังผู้ใช้และกลุ่มที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="1cd2f-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="1cd2f-108">ยืนยันว่าผู้ใช้กำลังใช้แอปที่รองรับป้ายความไว-ดูเล[เบลไวในเอกสารของคุณ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)</span><span class="sxs-lookup"><span data-stu-id="1cd2f-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="1cd2f-109">ถ้าคุณกำลัง[ย้ายป้ายชื่อการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)โปรดทราบถึงข้อควรพิจารณาที่ระบุไว้ที่[นี่](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)</span><span class="sxs-lookup"><span data-stu-id="1cd2f-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="1cd2f-110">การสนับสนุนการป้องกันการสูญหายของข้อมูล (DLP): ปัจจุบันเฉพาะป้ายเก็บข้อมูลเท่านั้นที่สามารถใช้เป็นเงื่อนไขในนโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="1cd2f-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="1cd2f-111">การสนับสนุนสำหรับป้ายความไวในนโยบาย DLP ยังไม่พร้อมใช้งานแต่เรากำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="1cd2f-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="1cd2f-112">เมื่อเปิดใช้งานการเข้ารหัสลับบนป้ายความไวคุณสามารถเลือกที่จะ:</span><span class="sxs-lookup"><span data-stu-id="1cd2f-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="1cd2f-113">กำหนดสิทธิ์ในขณะนี้</span><span class="sxs-lookup"><span data-stu-id="1cd2f-113">Assign permissions now</span></span>
    - <span data-ttu-id="1cd2f-114">ให้ผู้ใช้กำหนดสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="1cd2f-114">Let users assign permissions</span></span>


<span data-ttu-id="1cd2f-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับปัญหาที่เป็นไปได้โปรดดู[ปัญหาที่ทราบด้วยป้ายความไว](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)</span><span class="sxs-lookup"><span data-stu-id="1cd2f-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>