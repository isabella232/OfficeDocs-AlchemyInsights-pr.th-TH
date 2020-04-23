---
title: การโอนย้ายโดเมน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "4985"
ms.openlocfilehash: e78b560329254f7035869c076db5ff31427dc7ae
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43783990"
---
# <a name="domain-transfers"></a><span data-ttu-id="ee547-102">การโอนย้ายโดเมน</span><span class="sxs-lookup"><span data-stu-id="ee547-102">Domain transfers</span></span>

- <span data-ttu-id="ee547-103">[วิธีการถ่ายโอนโดเมนไมโครซอฟท์ซื้อไปยังผู้ให้บริการอื่นหลังจาก 60 วัน](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)</span><span class="sxs-lookup"><span data-stu-id="ee547-103">[How to transfer a Microsoft purchased domain to another provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq?view=o365-worldwide#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>

    - <span data-ttu-id="ee547-104">แม้ว่า Microsoft โดเมนที่ซื้อแล้วจะไม่สนับสนุนการเปลี่ยนแปลงระเบียน NS แต่ให้[ปรับปรุงระเบียน DNS สําหรับเว็บไซต์ของคุณ](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide)แทนที่จะถ่ายโอนการลงทะเบียนโดเมนของคุณไปยังเว็บโฮสต์</span><span class="sxs-lookup"><span data-stu-id="ee547-104">Although Microsoft purchased domains don't support changing NS records, consider [updating DNS records for your website](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider?view=o365-worldwide) instead of transferring your domain registration to the web hoster.</span></span>

- <span data-ttu-id="ee547-105">ไม่สามารถถ่ายโอนโดเมนที่ซื้อของ Microsoft ระหว่างผู้เช่า Microsoft 365 ได้</span><span class="sxs-lookup"><span data-stu-id="ee547-105">A Microsoft purchased domain cannot be transferred between Microsoft 365 tenants.</span></span> 

    - <span data-ttu-id="ee547-106">อย่างไรก็ตาม คุณสามารถถ่ายโอนโดเมนของบริษัทอื่นระหว่างผู้เช่า Microsoft 365 โดยการ[เอาโดเมนจากผู้เช่าหนึ่ง](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide)แล้ว ตรวจสอบโดเมนในผู้เช่าอื่น</span><span class="sxs-lookup"><span data-stu-id="ee547-106">However, you can transfer a third-party domain between Microsoft 365 tenants by [removing the domain from one tenant](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain?view=o365-worldwide) and then verifying the domain in another tenant.</span></span>

- <span data-ttu-id="ee547-107">การลงทะเบียนโดเมนหรือการเรียกเก็บเงินของบุคคลที่สามไม่สามารถโอนไปยัง Microsoft ได้</span><span class="sxs-lookup"><span data-stu-id="ee547-107">A third-party domains registration or billing cannot be transferred to Microsoft.</span></span>

    - <span data-ttu-id="ee547-108">แต่โดเมนแบบกําหนดเองสามารถ[ตรวจสอบและใช้กับ Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ee547-108">But custom domains can be  [verified and used with Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain?view=o365-worldwide).</span></span>

- <span data-ttu-id="ee547-109">Onmicrosoft.comโดเมนเริ่มต้นเริ่มต้นไม่สามารถถ่ายโอนหรือเปลี่ยนชื่อได้</span><span class="sxs-lookup"><span data-stu-id="ee547-109">Onmicrosoft.com initial default domains cannot be transferred or renamed.</span></span>
