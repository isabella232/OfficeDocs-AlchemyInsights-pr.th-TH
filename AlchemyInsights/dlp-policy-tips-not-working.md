---
title: DLP เคล็ดลับนโยบายที่ไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 9b3981964b66eb1c8083a3acf5ca31be3c8157fe
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389524"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="ea910-102">คำแนะนำนโยบาย DLP การตัดสินค้าจากคลัง</span><span class="sxs-lookup"><span data-stu-id="ea910-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="ea910-103">เมื่อใช้**นโยบาย DLP**ผู้ใช้สามารถได้รับการแจ้งของการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="ea910-103">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="ea910-104">ผู้ดูแลระบบสามารถกำหนดค่านโยบายเคล็ดลับเมื่อต้องการแสดงใน ขณะที่การทดสอบของนโยบาย DLP หรือนโยบายอยู่ในโหมดเต็มรูปแบบบังคับ</span><span class="sxs-lookup"><span data-stu-id="ea910-104">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="ea910-105">เมื่อต้องการตั้งค่าคอนฟิกนโยบายเคล็ดลับบนนโยบาย DLP ของคุณในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบในโหมดเต็มรูปแบบบังคับ ทำต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ea910-105">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="ea910-106">ให้แน่ใจว่า กฎ DLP โดยใช้ขั้นตอน**การเปิดใช้งาน**เคล็ดลับนโยบายได้[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="ea910-106">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="ea910-107">ให้แน่ใจว่าของคุณที่**ตรงกับเนื้อหา**คืออะไร**จำเป็นต้องใช้**เพื่อทริกเกอร์กฎต่าง ๆ ที่ระบุไว้ในบทความนี้[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ea910-107">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ea910-108">แสดงเคล็ดลับนโยบายทั้งใน OWA และ Outlook</span><span class="sxs-lookup"><span data-stu-id="ea910-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="ea910-109">อย่างไรก็ตาม เมื่อใช้**Outlook รุ่นที่ใหม่กว่า หรือ 2013**เคล็ดลับนโยบายจะแสดงขึ้นภายใต้เงื่อนไขบางอย่าง</span><span class="sxs-lookup"><span data-stu-id="ea910-109">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="ea910-110">เงื่อนไขเหล่านี้จะแสดงรายการอยู่ที่นี่:[เงื่อนไข Supported 2013 Outlook หรือรุ่นที่ใหม่กว่า สำหรับการแสดงเคล็ดลับนโยบาย](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="ea910-110">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="ea910-111">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับคำแนะนำนโยบาย DLP ดู:[แสดงคำแนะนำนโยบายสำหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="ea910-111">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  