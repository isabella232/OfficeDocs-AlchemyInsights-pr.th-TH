---
title: เคล็ดลับนโยบาย DLP ไม่ทํางาน
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
ms.openlocfilehash: 6375fa8077529f36ae95d6632ad4d2db5625dc29
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977253"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="7f89d-102">ปัญหาคําแนะนํานโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="7f89d-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="7f89d-103">**สําคัญ**: ในช่วงเวลาที่ไม่เคยมีมาก่อนเหล่านี้ เราจะดําเนินการเพื่อให้แน่ใจว่า SharePoint Online และบริการ OneDrive ยังคงพร้อมใช้งานสูง – โปรดเยี่ยมชม[SharePoint Online ชั่วคราวปรับปรุงคุณลักษณะชั่วคราว](https://aka.ms/ODSPAdjustments)สําหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="7f89d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="7f89d-104">**เคล็ดลับนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="7f89d-104">**DLP policy tips**</span></span>

<span data-ttu-id="7f89d-105">เมื่อใช้**นโยบาย DLP**ผู้ใช้จะได้รับการแจ้งเตือนเกี่ยวกับการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="7f89d-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="7f89d-106">ผู้ดูแลระบบสามารถกําหนดค่าคําแนะนํานโยบายให้แสดงขณะทดสอบนโยบาย DLP ของตน หรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้แบบเต็ม</span><span class="sxs-lookup"><span data-stu-id="7f89d-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="7f89d-107">เมื่อต้องการกําหนดค่านโยบายเคล็ดลับนโยบายนโยบาย DLP ของคุณในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามกฎระเบียบในโหมดการบังคับใช้แบบเต็ม ให้ทําดังนี้</span><span class="sxs-lookup"><span data-stu-id="7f89d-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="7f89d-108">ตรวจสอบให้แน่ใจว่าได้**เปิดใช้งาน**เคล็ดลับนโยบายในกฎ DLP โดยใช้ขั้นตอน[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="7f89d-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="7f89d-109">ตรวจสอบให้แน่ใจ**ว่าเนื้อหาของคุณตรงกับ\*\*\*\*สิ่งที่จําเป็น**เพื่อทริกเกอร์กฎที่กล่าวถึงในบทความนี้[ที่นี่](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7f89d-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="7f89d-110">คําแนะนํานโยบายแสดงทั้งใน OWA และ Outlook</span><span class="sxs-lookup"><span data-stu-id="7f89d-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="7f89d-111">อย่างไรก็ตาม เมื่อใช้**Outlook 2013 หรือรุ่นที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="7f89d-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="7f89d-112">เงื่อนไขเหล่านี้จะแสดงอยู่ที่นี่:[เงื่อนไขที่ได้รับการสนับสนุนสําหรับ Outlook 2013 หรือรุ่นที่ใหม่กว่าสําหรับการแสดงคําแนะนํานโยบาย](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="7f89d-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="7f89d-113">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ให้ดูที่:[แสดงเคล็ดลับนโยบายสําหรับนโยบาย DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="7f89d-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  