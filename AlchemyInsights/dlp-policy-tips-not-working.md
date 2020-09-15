---
title: เคล็ดลับนโยบาย DLP ไม่ทำงาน
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679604"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="61604-102">ปัญหาเกี่ยวกับเคล็ดลับนโยบาย DLP</span><span class="sxs-lookup"><span data-stu-id="61604-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="61604-103">**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="61604-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="61604-104">**เคล็ดลับนโยบาย DLP**</span><span class="sxs-lookup"><span data-stu-id="61604-104">**DLP policy tips**</span></span>

<span data-ttu-id="61604-105">เมื่อใช้**นโยบาย DLP**ผู้ใช้สามารถได้รับการแจ้งให้ทราบเกี่ยวกับการละเมิดนโยบายด้วย**เคล็ดลับนโยบาย**</span><span class="sxs-lookup"><span data-stu-id="61604-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="61604-106">ผู้ดูแลระบบสามารถกำหนดค่าเคล็ดลับนโยบายในการแสดงในขณะที่ทดสอบนโยบาย DLP ของพวกเขาหรือเมื่อนโยบายอยู่ในโหมดการบังคับใช้แบบเต็ม</span><span class="sxs-lookup"><span data-stu-id="61604-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="61604-107">เมื่อต้องการกำหนดค่าเคล็ดลับนโยบายในนโยบาย DLP ของคุณในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายในโหมดการบังคับใช้แบบเต็มให้ทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="61604-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="61604-108">ตรวจสอบให้แน่ใจว่ามีการ**เปิดใช้งาน**เคล็ดลับนโยบายในกฎ DLP โดยใช้ขั้นตอน[ต่อไปนี้](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="61604-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="61604-109">ตรวจสอบให้แน่ใจว่าเนื้อหาของคุณ**ตรงกับ**สิ่งที่จำเป็นต้อง**ใช้**ในการทริกเกอร์กฎที่ระบุไว้ในบทความนี้[ที่นี่](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="61604-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="61604-110">เคล็ดลับนโยบายแสดงในทั้ง OWA และ Outlook</span><span class="sxs-lookup"><span data-stu-id="61604-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="61604-111">อย่างไรก็ตามเมื่อใช้ **Outlook ๒๐๑๓หรือใหม่กว่า**คำแนะนำนโยบายจะแสดงเฉพาะภายใต้เงื่อนไขบางอย่าง</span><span class="sxs-lookup"><span data-stu-id="61604-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="61604-112">เงื่อนไขเหล่านี้จะแสดงรายการที่นี่: เงื่อนไขที่ได้ [รับการสนับสนุนสำหรับ Outlook ๒๐๑๓หรือใหม่กว่าสำหรับการแสดงเคล็ดลับนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="61604-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="61604-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับเคล็ดลับนโยบาย DLP ให้ดูที่: [แสดงเคล็ดลับนโยบายสำหรับนโยบาย DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="61604-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  