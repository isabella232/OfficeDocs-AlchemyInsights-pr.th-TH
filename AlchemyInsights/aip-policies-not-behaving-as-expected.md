---
title: 'AIP: นโยบายไม่ทํางานตามที่คาดไว้'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580784"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="9aeb8-102">AIP: นโยบายไม่ทํางานตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="9aeb8-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="9aeb8-103">การป้องกันข้อมูล azure: นโยบายไม่ทํางานตามที่คาดไว้ ให้ดูคําแนะนําต่อไปนี้สําหรับปัญหานโยบายต่าง ๆ:</span><span class="sxs-lookup"><span data-stu-id="9aeb8-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="9aeb8-104">หากคุณมีปัญหากับการทําเครื่องหมายภาพ โปรดตรวจทาน[เมื่อมีใช้เครื่องหมายภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="9aeb8-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="9aeb8-105">ถ้าคุณกําลังมีปัญหากับการติดฉลากอัตโนมัติ โปรดดู[วิธีการกําหนดค่าเงื่อนไขสําหรับการจัดประเภทอัตโนมัติและแนะนําสําหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ชนิดของข้อมูลที่ละเอียดอ่อนจะมีลักษณะอย่างไร](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9aeb8-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="9aeb8-106">หากคุณมีปัญหากับการป้องกันเนทีฟ / Pfile โปรดตรวจสอบ[การกําหนดค่าไฟล์ API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="9aeb8-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="9aeb8-107">ตรวจสอบว่า คุณกําลังใช้นโยบายขอบเขตที่ไม่ได้ถูกกําหนดค่าอย่างถูกต้อง:[วิธีการตั้งค่าคอนฟิกนโยบายการป้องกันข้อมูล Azure สําหรับผู้ใช้เฉพาะ โดยใช้นโยบายขอบเขต](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="9aeb8-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="9aeb8-108">ถ้าการติดฉลากอัตโนมัติไม่ทํางานสําหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อ ให้ตรวจสอบว่าไม่ได้กําหนด DRMEncryptProperty ตามที่อธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM เพื่อความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="9aeb8-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="9aeb8-109">ถ้าคุณยังคงประสบปัญหา โปรดรวบรวมแฟ้มบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบแฟ้มบันทึกที่ส่งออกไปยังใบสั่งงานนี้</span><span class="sxs-lookup"><span data-stu-id="9aeb8-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="9aeb8-110">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="9aeb8-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="9aeb8-111">คลิก**Protect/Sensitivity**  >  **วิธีใช้และคําติชม**ป้องกัน/ความไว</span><span class="sxs-lookup"><span data-stu-id="9aeb8-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="9aeb8-112">คลิก**ส่งออกแฟ้มบันทึก**</span><span class="sxs-lookup"><span data-stu-id="9aeb8-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="9aeb8-113">บันทึกบันทึกไปยังตําแหน่งที่ตั้งที่คุณเลือก และแนบไฟล์เหล่านั้นกับคําขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="9aeb8-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="9aeb8-114">ทรัพยากรเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="9aeb8-114">Additional resources:</span></span>

- [<span data-ttu-id="9aeb8-115">วิธีการกําหนดค่าป้ายชื่อสําหรับเครื่องหมายภาพสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="9aeb8-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="9aeb8-116">ตรวจทานเอกสารการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="9aeb8-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9aeb8-117">ใช้ป้ายชื่อความไวในแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9aeb8-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

