---
title: ความขัดแย้งกับ SourceAnchor, พร็อกซีที่อยู่, ชื่อผู้ใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198576"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="3d392-102">ความขัดแย้งกับ SourceAnchor, พร็อกซีที่อยู่, ชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3d392-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="3d392-103">ถ้าคุณได้รับข้อผิดพลาดในระหว่างการซิงโครไนส์ เช่น "วัตถุที่ซิงโครไนส์กับ ProxyAddress เดียวกันหรือ UserPrincipalName เดียวกันอยู่ในไดเรกทอรีของคุณ" ให้ดู[วินิจฉัย และแก้ไขข้อผิดพลาดการซิงค์แอตทริบิวต์ที่ซ้ํากัน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)</span><span class="sxs-lookup"><span data-stu-id="3d392-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="3d392-104">นอกจากนี้ ให้พิจารณาการเปิดใช้งานความยืดหยุ่นของแอตทริบิวต์ที่ซ้ํากัน</span><span class="sxs-lookup"><span data-stu-id="3d392-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="3d392-105">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การซิงโครไนส์ข้อมูลประจําตัวและความยืดหยุ่นของแอตทริบิวต์ที่ซ้ํากัน](https://aka.ms/duplicateattributeresiliency)</span><span class="sxs-lookup"><span data-stu-id="3d392-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>