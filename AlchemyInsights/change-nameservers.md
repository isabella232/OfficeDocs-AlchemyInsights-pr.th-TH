---
title: เปลี่ยนเซิร์ฟเวอร์ชื่อ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818631"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="91a68-102">อัปเดตเนมเซิร์ฟเวอร์ของโดเมนให้ชี้ไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="91a68-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="91a68-103">หมายเหตุ: บางครั้งการเปลี่ยนแปลงเซิร์ฟเวอร์ชื่ออาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="91a68-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="91a68-104">เมื่อต้องการตั้งค่าโดเมนใน Microsoft 365 จะต้องอัปเดตเนมเซิร์ฟเวอร์ที่บริษัทจดทะเบียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="91a68-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="91a68-105">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="91a68-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="91a68-106">ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณ และค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้</span><span class="sxs-lookup"><span data-stu-id="91a68-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="91a68-107">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์สองระเบียนให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="91a68-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="91a68-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91a68-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="91a68-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91a68-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="91a68-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="91a68-110">Save changes.</span></span>

<span data-ttu-id="91a68-111">คุณยังสามารถค้นหาคําแนะนําโดยละเอียดในบทความนี้: [เปลี่ยนเนมเซิร์ฟเวอร์กับบริษัทจดทะเบียนโดเมน](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="91a68-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  