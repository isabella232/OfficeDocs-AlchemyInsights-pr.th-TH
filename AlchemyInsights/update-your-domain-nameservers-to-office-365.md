---
title: ปรับปรุงเซิร์ฟเวอร์โดเมนของคุณให้ชี้ไปที่ไมโครซอฟท์
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720012"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="53c4a-102">ปรับปรุงเซิร์ฟเวอร์โดเมนของคุณให้ชี้ไปที่ไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="53c4a-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="53c4a-103">หมายเหตุ: การเปลี่ยนแปลงเนมเซิร์ฟเวอร์อาจใช้เวลาถึง 48 ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="53c4a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="53c4a-104">เมื่อต้องการตั้งค่าโดเมนของคุณกับ Microsoft เนมเซิร์ฟเวอร์ที่นายทะเบียนของคุณจําเป็นต้องได้รับการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="53c4a-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="53c4a-105">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="53c4a-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="53c4a-106">ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนและค้นหาพื้นที่ที่คุณสามารถแก้ไขเนมเซิร์ฟเวอร์ได้</span><span class="sxs-lookup"><span data-stu-id="53c4a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="53c4a-107">สร้างหรือแก้ไขระเบียนเนมเซิร์ฟเวอร์สองระเบียนเพื่อให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="53c4a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="53c4a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="53c4a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="53c4a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="53c4a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="53c4a-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="53c4a-110">Save changes.</span></span>

<span data-ttu-id="53c4a-111">คุณยังสามารถค้นหาคําแนะนําโดยละเอียดในบทความนี้:[เปลี่ยนเนมเซิร์ฟเวอร์เพื่อตั้งค่า Microsoft 365 กับบริษัทจดทะเบียนโดเมนใดๆ](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="53c4a-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  