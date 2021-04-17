---
title: 'AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้'
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
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821718"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="24ff3-102">AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="24ff3-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="24ff3-103">ถ้าคุณพบปัญหาเกี่ยวกับเครื่องหมายแบบเป็นภาพไม่แสดงตามที่คาดไว้ ให้ดูแนวทางต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="24ff3-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="24ff3-104">ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทานแล้ว [เมื่อมีการใช้เครื่องหมายแบบ](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)เป็นภาพ</span><span class="sxs-lookup"><span data-stu-id="24ff3-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="24ff3-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span><span class="sxs-lookup"><span data-stu-id="24ff3-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="24ff3-106">ถ้าคุณต้องการเอาหัวกระดาษ/ท้ายกระดาษที่มีอยู่ออก ให้ตรวจทาน [เอาหัวกระดาษและท้ายกระดาษออกจากโซลูชันการติดป้ายชื่อ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)อื่นๆ</span><span class="sxs-lookup"><span data-stu-id="24ff3-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="24ff3-107">ถ้าคุณยังคงพบปัญหานี้ ให้รวบรวมบันทึกของไคลเอ็นต์ Azure Information Protection และแนบบันทึกที่ส่งออกไปยังตั๋วนี้</span><span class="sxs-lookup"><span data-stu-id="24ff3-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="24ff3-108">**ส่งออกบันทึก Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="24ff3-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="24ff3-109">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="24ff3-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="24ff3-110">คลิก **วิธีใช้และข้อคิดเห็นเกี่ยวกับการป้องกัน/** ระดับ  >  **ความลับ**</span><span class="sxs-lookup"><span data-stu-id="24ff3-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="24ff3-111">คลิก **ส่งออก** แฟ้มบันทึก</span><span class="sxs-lookup"><span data-stu-id="24ff3-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="24ff3-112">บันทึกแฟ้มบันทึกไปยังตัวเลือกของสถานที่และแนบไฟล์ไปกับการร้องขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="24ff3-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="24ff3-113">โปรดดูข้อมูลเพิ่มเติมที่:</span><span class="sxs-lookup"><span data-stu-id="24ff3-113">For additional information, see:</span></span>

- [<span data-ttu-id="24ff3-114">วิธีการกําหนดค่าป้ายชื่อเพื่อเครื่องหมายแบบเป็นภาพเพื่อ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="24ff3-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="24ff3-115">ตรวจทานเอกสาร Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="24ff3-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="24ff3-116">ความต้องการของ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="24ff3-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="24ff3-117">บทช่วยสอนเริ่มต้นใช้งานด่วนของ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="24ff3-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="24ff3-118">ดาวน์โหลดไคลเอ็นต์ Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="24ff3-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
