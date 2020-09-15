---
title: 'AIP: นโยบายที่ไม่ถูกต้องตามที่คาดไว้'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663208"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="96ac9-102">AIP: นโยบายที่ไม่ถูกต้องตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="96ac9-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="96ac9-103">การป้องกันข้อมูลของ Azure: นโยบายไม่มีลักษณะการใช้งานตามที่คาดไว้ให้ดูที่คำแนะนำที่แนะนำสำหรับปัญหานโยบายต่างๆดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="96ac9-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="96ac9-104">ถ้าคุณกำลังมีปัญหาเกี่ยวกับการทำเครื่องหมายการมองเห็นโปรดตรวจทานเมื่อมีการนำการทำเครื่องหมาย[แสดงผลไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="96ac9-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="96ac9-105">ถ้าคุณกำลังมีปัญหาเกี่ยวกับการติดป้ายอัตโนมัติโปรดตรวจทาน[วิธีการกำหนดค่าเงื่อนไขสำหรับการจัดประเภทโดยอัตโนมัติและที่แนะนำสำหรับการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)และ[ลักษณะที่ปรากฏของชนิดข้อมูลที่ละเอียดอ่อน](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="96ac9-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="96ac9-106">ถ้าคุณกำลังมีปัญหาเกี่ยวกับการป้องกันพื้นเมือง/Pfile โปรดตรวจทาน[การกำหนดค่า API ของไฟล์](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="96ac9-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="96ac9-107">ตรวจสอบว่าคุณกำลังใช้นโยบายลักษณะที่ไม่ได้รับการกำหนดค่าอย่างถูกต้อง:[วิธีการกำหนดค่านโยบายการป้องกันข้อมูล Azure สำหรับผู้ใช้ที่เฉพาะเจาะจงโดยใช้นโยบายลักษณะ](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="96ac9-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="96ac9-108">ถ้าการติดป้ายอัตโนมัติไม่ทำงานสำหรับ Outlook เมื่อแนบเอกสารที่มีป้ายชื่อให้ตรวจสอบว่า DRMEncryptProperty ไม่ได้ถูกกำหนดตามที่อธิบายไว้ที่นี่:[การตั้งค่ารีจิสทรี IRM สำหรับความปลอดภัย](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="96ac9-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="96ac9-109">ถ้าคุณยังคงพบปัญหาโปรดรวบรวมบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบไฟล์บันทึกที่ส่งออกไปยังตั๋วนี้</span><span class="sxs-lookup"><span data-stu-id="96ac9-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="96ac9-110">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="96ac9-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="96ac9-111">คลิกการ**ป้องกัน/ความไว**ต่อ  >  **วิธีใช้และคำติชม**</span><span class="sxs-lookup"><span data-stu-id="96ac9-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="96ac9-112">คลิก**ส่งออกบันทึก**</span><span class="sxs-lookup"><span data-stu-id="96ac9-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="96ac9-113">บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="96ac9-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="96ac9-114">แหล่งข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="96ac9-114">Additional resources:</span></span>

- [<span data-ttu-id="96ac9-115">วิธีการกำหนดค่าป้ายชื่อสำหรับเครื่องหมายภาพสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="96ac9-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="96ac9-116">ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="96ac9-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="96ac9-117">ใช้ป้ายความลับของแอป Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="96ac9-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

