---
title: อัปเดเซิร์ฟเวอร์ชื่อโดเมนของคุณให้ชี้ไปที่ Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734930"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="45c22-102">อัปเดเซิร์ฟเวอร์ชื่อโดเมนของคุณให้ชี้ไปที่ Microsoft</span><span class="sxs-lookup"><span data-stu-id="45c22-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="45c22-103">หมายเหตุ: การเปลี่ยนแปลง Nameserver บางครั้งอาจใช้เวลาถึง๔๘ชั่วโมงในการเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="45c22-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="45c22-104">เมื่อต้องการตั้งค่าโดเมนของคุณด้วย Microsoft การเซิร์ฟเวอร์ชื่อที่บริษัทจดทะเบียนของคุณจำเป็นต้องได้รับการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="45c22-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="45c22-105">สร้างหรือแก้ไขระเบียน nameserver ของคุณที่บริษัทจดทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="45c22-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="45c22-106">ไปที่เว็บไซต์ของบริษัทจดทะเบียนโดเมนของคุณและค้นหาพื้นที่ที่คุณสามารถแก้ไขเซิร์ฟเวอร์ชื่อได้</span><span class="sxs-lookup"><span data-stu-id="45c22-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="45c22-107">สร้างหรือแก้ไขระเบียน nameserver สองระเบียนให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="45c22-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="45c22-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="45c22-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="45c22-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="45c22-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="45c22-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="45c22-110">Save changes.</span></span>

<span data-ttu-id="45c22-111">นอกจากนี้คุณยังสามารถค้นหาคำแนะนำโดยละเอียดในบทความนี้:[เปลี่ยนเซิร์ฟเวอร์ชื่อเพื่อตั้งค่า Microsoft ๓๖๕กับบริษัทจดทะเบียนโดเมนใดก็](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)ได้</span><span class="sxs-lookup"><span data-stu-id="45c22-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  