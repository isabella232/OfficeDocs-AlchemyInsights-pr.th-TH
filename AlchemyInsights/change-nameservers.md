---
title: เปลี่ยน NameServers
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
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902948"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="03ca8-102">อัพเด nameservers โดเมนของคุณกับ Office 365</span><span class="sxs-lookup"><span data-stu-id="03ca8-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="03ca8-103">หมายเหตุ: เปลี่ยนแปลง Nameserver ในบางครั้งอาจถึง 48 ชั่วโมงเพื่อเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="03ca8-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="03ca8-104">เมื่อต้องการตั้งค่าโดเมนของคุณใน Office 365, nameservers หมายที่ผู้ลงทะเบียนของคุณต้องถูกปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="03ca8-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="03ca8-105">สร้าง หรือแก้ไขเรกคอร์ nameserver ของคุณที่ผู้ลงทะเบียนโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="03ca8-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="03ca8-106">ไปที่เว็บไซต์ของผู้ลงทะเบียนโดเมนของคุณ และค้นหาพื้นที่ซึ่งคุณสามารถแก้ไขการ nameservers</span><span class="sxs-lookup"><span data-stu-id="03ca8-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="03ca8-107">สร้าง หรือแก้ไขเรกคอร์ nameserver สองเพื่อให้ตรงกับค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="03ca8-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="03ca8-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="03ca8-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="03ca8-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="03ca8-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="03ca8-110">บันทึกการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="03ca8-110">Save changes.</span></span>

<span data-ttu-id="03ca8-111">คุณยังสามารถค้นหาคำแนะนำโดยละเอียดในบทความนี้: [nameservers การเปลี่ยนแปลงการตั้งค่า Office 365 กับผู้ลงทะเบียนโดเมนใด ๆ](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="03ca8-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  