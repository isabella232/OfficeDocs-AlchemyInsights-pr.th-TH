---
title: เปลี่ยนเซิร์ฟเวอร์ชื่อ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508107"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ca31d-102">อัปเดตเซิร์ฟเวอร์ชื่อโดเมนของคุณให้ชี้ไปที่ Microsoft</span><span class="sxs-lookup"><span data-stu-id="ca31d-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ca31d-103">หมายเหตุ: บางครั้งการเปลี่ยนแปลงเนมเซิร์ฟเวอร์อาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="ca31d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ca31d-104">เมื่อต้องการตั้งค่าโดเมนของคุณใน Microsoft 365 เนมเซิร์ฟเวอร์ที่นายทะเบียนของคุณต้องได้รับการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="ca31d-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ca31d-105">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="ca31d-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ca31d-106">ไปที่เว็บไซต์ของผู้รับจดทะเบียนโดเมนและค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้</span><span class="sxs-lookup"><span data-stu-id="ca31d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="ca31d-107">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์สองระเบียนให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="ca31d-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ca31d-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca31d-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ca31d-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca31d-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ca31d-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="ca31d-110">Save changes.</span></span>

<span data-ttu-id="ca31d-111">นอกจากนี้คุณยังสามารถค้นหาคําแนะนําโดยละเอียดในบทความนี้:[เปลี่ยนเนมเซิร์ฟเวอร์กับผู้รับจดทะเบียนโดเมนใด ๆ](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ca31d-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  