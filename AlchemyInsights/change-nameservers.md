---
title: เปลี่ยนเนมเซิร์ฟเวอร์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736668"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="89f8c-102">ปรับปรุงเซิร์ฟเวอร์โดเมนของคุณให้เป็น Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="89f8c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="89f8c-103">หมายเหตุ: บางครั้งการเปลี่ยนแปลงเนมเซิร์ฟเวอร์อาจใช้เวลาถึง๔๘ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="89f8c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="89f8c-104">เมื่อต้องการตั้งค่าโดเมนของคุณใน Office ๓๖๕เนมเซิร์ฟเวอร์ที่นายทะเบียนของคุณจำเป็นต้องได้รับการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="89f8c-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="89f8c-105">สร้างหรือแก้ไขเรกคอร์ดเนมเซิร์ฟเวอร์ที่นายทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="89f8c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="89f8c-106">ไปที่เว็บไซต์ของผู้รับจดทะเบียนโดเมนของคุณและค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้</span><span class="sxs-lookup"><span data-stu-id="89f8c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="89f8c-107">สร้างหรือแก้ไขเรกคอร์ดที่สองเนมเซิร์ฟเวอร์เพื่อให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="89f8c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="89f8c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="89f8c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="89f8c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="89f8c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="89f8c-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="89f8c-110">Save changes.</span></span>

<span data-ttu-id="89f8c-111">นอกจากนี้คุณยังสามารถค้นหาคำแนะนำโดยละเอียดในบทความนี้:[เปลี่ยนเนมเซิร์ฟเวอร์เพื่อตั้งค่า Office ๓๖๕กับผู้รับจดทะเบียนโดเมนใดๆ](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="89f8c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  