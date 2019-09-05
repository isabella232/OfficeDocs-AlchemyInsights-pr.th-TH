---
title: ปรับปรุงเซิร์ฟเวอร์โดเมนของคุณให้เป็น Office ๓๖๕
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742207"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="af6fd-102">ปรับปรุงเซิร์ฟเวอร์โดเมนของคุณให้เป็น Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="af6fd-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="af6fd-103">หมายเหตุ: บางครั้งการเปลี่ยนแปลงเนมเซิร์ฟเวอร์อาจใช้เวลาถึง๔๘ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="af6fd-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="af6fd-104">เมื่อต้องการตั้งค่าโดเมนของคุณใน Office ๓๖๕เนมเซิร์ฟเวอร์ที่นายทะเบียนของคุณจำเป็นต้องได้รับการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="af6fd-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="af6fd-105">สร้างหรือแก้ไขเรกคอร์ดเนมเซิร์ฟเวอร์ที่นายทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="af6fd-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="af6fd-106">ไปที่เว็บไซต์ของผู้รับจดทะเบียนโดเมนของคุณและค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้</span><span class="sxs-lookup"><span data-stu-id="af6fd-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="af6fd-107">สร้างหรือแก้ไขเรกคอร์ดที่สองเนมเซิร์ฟเวอร์เพื่อให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="af6fd-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="af6fd-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af6fd-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="af6fd-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af6fd-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="af6fd-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="af6fd-110">Save changes.</span></span>

<span data-ttu-id="af6fd-111">นอกจากนี้คุณยังสามารถค้นหาคำแนะนำโดยละเอียดในบทความนี้:[เปลี่ยนเนมเซิร์ฟเวอร์เพื่อตั้งค่า Office ๓๖๕กับผู้รับจดทะเบียนโดเมนใดๆ](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="af6fd-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  