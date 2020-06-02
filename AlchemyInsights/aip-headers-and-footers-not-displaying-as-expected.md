---
title: 'AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้'
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
- "4541"
ms.openlocfilehash: 418362beea221a7cb9d8fd4be6cfc0f28022093d
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493409"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="c32ef-102">AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="c32ef-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="c32ef-103">ถ้าคุณประสบปัญหาเกี่ยวกับการทําเครื่องหมายภาพไม่แสดงตามที่คาดไว้ ให้ดูแนวทางต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="c32ef-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="c32ef-104">ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทาน[เมื่อมีการใช้เครื่องหมายภาพ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="c32ef-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="c32ef-105">สําหรับการติดฉลาก Office ให้ตรวจทาน[เมื่อ Office 365 ใช้การทําเครื่องหมายเนื้อหาและการเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)</span><span class="sxs-lookup"><span data-stu-id="c32ef-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="c32ef-106">ถ้าคุณต้องการเอาหัวกระดาษ/ท้ายกระดาษที่มีอยู่ออก ให้[ตรวจทาน เอาหัวกระดาษและท้ายกระดาษออกจากโซลูชันการติดฉลากอื่นๆ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)</span><span class="sxs-lookup"><span data-stu-id="c32ef-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="c32ef-107">ถ้าคุณยังคงประสบปัญหา ให้เก็บรวบรวมแฟ้มบันทึกของไคลเอ็นต์การป้องกันข้อมูล Azure และแนบแฟ้มบันทึกที่ส่งออกไปยังใบสั่งงานนี้</span><span class="sxs-lookup"><span data-stu-id="c32ef-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="c32ef-108">**ส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="c32ef-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="c32ef-109">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="c32ef-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="c32ef-110">คลิก**Protect/Sensitivity**  >  **วิธีใช้และคําติชม**ป้องกัน/ความไว</span><span class="sxs-lookup"><span data-stu-id="c32ef-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="c32ef-111">คลิก**ส่งออกแฟ้มบันทึก**</span><span class="sxs-lookup"><span data-stu-id="c32ef-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="c32ef-112">บันทึกบันทึกไปยังตําแหน่งที่ตั้งที่คุณเลือก และแนบไฟล์เหล่านั้นกับคําขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="c32ef-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="c32ef-113">สําหรับข้อมูลเพิ่มเติม โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="c32ef-113">For additional information, see:</span></span>

- [<span data-ttu-id="c32ef-114">วิธีการกําหนดค่าป้ายชื่อสําหรับเครื่องหมายภาพสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="c32ef-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="c32ef-115">ตรวจทานเอกสารการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="c32ef-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c32ef-116">ข้อกําหนดสําหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="c32ef-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c32ef-117">บทช่วยสอนเริ่มต้นใช้งานอย่างย่อสําหรับการปกป้องข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="c32ef-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="c32ef-118">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="c32ef-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
