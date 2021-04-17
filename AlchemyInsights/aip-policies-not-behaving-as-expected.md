---
title: 'AIP: นโยบายไม่เป็นไปตามที่คาดไว้'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821646"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="69803-102">AIP: นโยบายไม่เป็นไปตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="69803-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="69803-103">Azure Information Protection: นโยบายไม่เป็นไปตามที่คาดไว้ ให้ดูรายการต่อไปนี้เพื่อดูแนวทางที่แนะนําเกี่ยวกับปัญหาต่างๆ ของนโยบาย:</span><span class="sxs-lookup"><span data-stu-id="69803-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="69803-104">ถ้าคุณมีปัญหากับการมาร์กอัปแบบเป็นภาพ โปรดตรวจสอบ[เมื่อมีการใช้เครื่องหมายด้วยภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="69803-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="69803-105">ถ้าคุณมีปัญหากับการกําหนดป้ายชื่ออัตโนมัติ โปรดดู วิธีการกําหนดค่าเงื่อนไขเพื่อการจัดประเภทอัตโนมัติและแนะนาเกี่ยวกับ [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) และ ชนิดข้อมูลที่เป็นความลับ [มีลักษณะ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)อย่างไร</span><span class="sxs-lookup"><span data-stu-id="69803-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="69803-106">ถ้าคุณมีปัญหากับการป้องกัน Native/Pfile โปรดตรวจสอบ การกําหนด [ค่า API ของ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)ไฟล์</span><span class="sxs-lookup"><span data-stu-id="69803-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="69803-107">ตรวจสอบว่าคุณใช้นโยบายขอบเขตที่กําหนดค่าไม่ถูกต้องหรือไม่: วิธีกําหนดค่านโยบาย[Azure Information Protection ของผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายที่กําหนดขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="69803-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="69803-108">ถ้าการกําหนดป้ายชื่ออัตโนมัติไม่ใช้งานกับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่า DRMEncryptProperty ไม่ได้กําหนดไว้ตามที่อธิบายไว้ที่นี่: การตั้งค่ารีจิสทรี[IRM เพื่อความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="69803-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="69803-109">ถ้าคุณยังคงพบปัญหา โปรดรวบรวมบันทึกของไคลเอ็นต์ Azure Information Protection และแนบบันทึกที่ส่งออกไปยังตั๋วนี้</span><span class="sxs-lookup"><span data-stu-id="69803-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="69803-110">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="69803-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="69803-111">คลิก **วิธีใช้และข้อคิดเห็นเกี่ยวกับการป้องกัน/** ระดับ  >  **ความลับ**</span><span class="sxs-lookup"><span data-stu-id="69803-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="69803-112">คลิก **ส่งออก** แฟ้มบันทึก</span><span class="sxs-lookup"><span data-stu-id="69803-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="69803-113">บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์ไปกับการร้องขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="69803-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="69803-114">แหล่งข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="69803-114">Additional resources:</span></span>

- [<span data-ttu-id="69803-115">วิธีการกําหนดค่าป้ายชื่อเพื่อเครื่องหมายแบบเป็นภาพเพื่อ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="69803-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="69803-116">ตรวจทานเอกสาร Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="69803-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="69803-117">ใช้ป้ายชื่อระดับความลับในแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="69803-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

