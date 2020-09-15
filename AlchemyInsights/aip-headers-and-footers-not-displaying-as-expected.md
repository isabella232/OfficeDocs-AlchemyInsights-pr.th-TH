---
title: 'AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้'
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
- "4541"
ms.openlocfilehash: 811a48587272776c8ece5e654a921c15cf52af5f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696567"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="f1ece-102">AIP: หัวกระดาษและท้ายกระดาษไม่แสดงตามที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="f1ece-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="f1ece-103">ถ้าคุณพบปัญหาเกี่ยวกับการทำเครื่องหมายการแสดงผลที่ไม่แสดงตามที่คาดไว้ให้ดูแนวทางต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f1ece-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="f1ece-104">ตรวจสอบให้แน่ใจว่าคุณได้รับการตรวจทาน[เมื่อมีการนำเครื่องหมายภาพไปใช้](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="f1ece-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f1ece-105">สำหรับการติดป้าย Office ให้ตรวจทาน[เมื่อ office ๓๖๕ใช้การทำเครื่องหมายเนื้อหาและการเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)</span><span class="sxs-lookup"><span data-stu-id="f1ece-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="f1ece-106">ถ้าคุณต้องการเอาส่วนหัว/ส่วนท้ายที่มีอยู่ออกให้รีวิว[เอาหัวกระดาษและท้ายกระดาษออกจากโซลูชันการติดฉลากอื่นๆ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)</span><span class="sxs-lookup"><span data-stu-id="f1ece-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="f1ece-107">ถ้าคุณยังคงพบปัญหาให้รวบรวมล็อกไคลเอ็นต์การป้องกันข้อมูลของ Azure และแนบไฟล์บันทึกที่ส่งออกไปยังตั๋วนี้</span><span class="sxs-lookup"><span data-stu-id="f1ece-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="f1ece-108">**ส่งออกแฟ้มบันทึกการป้องกันข้อมูล Azure**</span><span class="sxs-lookup"><span data-stu-id="f1ece-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="f1ece-109">เปิดเอกสาร Office หรือสร้างอีเมลใหม่ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="f1ece-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f1ece-110">คลิกการ**ป้องกัน/ความไว**ต่อ  >  **วิธีใช้และคำติชม**</span><span class="sxs-lookup"><span data-stu-id="f1ece-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f1ece-111">คลิก**ส่งออกบันทึก**</span><span class="sxs-lookup"><span data-stu-id="f1ece-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f1ece-112">บันทึกไฟล์บันทึกไปยังตำแหน่งที่ตั้งของคุณและแนบเข้ากับคำขอบริการนี้</span><span class="sxs-lookup"><span data-stu-id="f1ece-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f1ece-113">สำหรับข้อมูลเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="f1ece-113">For additional information, see:</span></span>

- [<span data-ttu-id="f1ece-114">วิธีการกำหนดค่าป้ายชื่อสำหรับเครื่องหมายภาพสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="f1ece-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f1ece-115">ตรวจทานเอกสารประกอบการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="f1ece-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f1ece-116">ข้อกำหนดสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="f1ece-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="f1ece-117">บทช่วยสอนเริ่มต้นใช้งานด่วนสำหรับการป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="f1ece-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="f1ece-118">ดาวน์โหลดไคลเอ็นต์การป้องกันข้อมูล Azure</span><span class="sxs-lookup"><span data-stu-id="f1ece-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
