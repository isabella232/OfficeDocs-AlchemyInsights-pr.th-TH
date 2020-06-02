---
title: เคล็ดลับนโยบาย DLP ไม่ทํางาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 9369878b62a5abe79bd215487bea6cabb0e80f06
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507461"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="5d53d-102">ปัญหาคําแนะนําเกี่ยวกับนโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="5d53d-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="5d53d-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้เรากําลังดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงมีอยู่มาก - โปรดเยี่ยมชม[SharePoint ออนไลน์ชั่วคราวการปรับปรุงคุณลักษณะ](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="5d53d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5d53d-104">**เคล็ดลับนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="5d53d-104">**DLP policy tips**</span></span>

<span data-ttu-id="5d53d-105">เมื่อใช้**นโยบาย DLP**ผู้ใช้สามารถได้รับแจ้งการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="5d53d-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="5d53d-106">ผู้ดูแลระบบสามารถกําหนดค่าเคล็ดลับนโยบายเพื่อแสดงในขณะที่ทดสอบนโยบาย DLP หรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้เต็มรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="5d53d-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="5d53d-107">เมื่อต้องการกําหนดค่าคําแนะนําด้านนโยบายเกี่ยวกับนโยบาย DLP ของคุณในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบในโหมดการบังคับใช้เต็มรูปแบบ ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="5d53d-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="5d53d-108">ตรวจสอบให้แน่ใจว่าได้**เปิดใช้งาน**เคล็ดลับนโยบายบนกฎ DLP โดยใช้ขั้นตอน[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="5d53d-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="5d53d-109">ให้แน่ใจว่า**เนื้อหาของคุณตรงกับ**สิ่งที่**ต้อง**เรียกกฎที่ระบุไว้ในบทความนี้[here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5d53d-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="5d53d-110">เคล็ดลับนโยบายแสดงใน OWA และ Outlook</span><span class="sxs-lookup"><span data-stu-id="5d53d-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="5d53d-111">อย่างไรก็ตาม เมื่อใช้**Outlook 2013 หรือใหม่กว่า**เคล็ดลับนโยบายจะแสดงภายใต้เงื่อนไขบางอย่างเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="5d53d-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="5d53d-112">เงื่อนไขเหล่านี้แสดงอยู่ที่นี่:[เงื่อนไขที่ได้รับการสนับสนุนสําหรับ Outlook 2013 หรือรุ่นที่ใหม่กว่าสําหรับการแสดงเคล็ดลับนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="5d53d-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="5d53d-113">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ดู:[แสดงเคล็ดลับนโยบายสําหรับนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="5d53d-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  