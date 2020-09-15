---
title: ข้อขัดแย้งกับ SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713473"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="e08dc-102">ข้อขัดแย้งกับ SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e08dc-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="e08dc-103">ถ้าคุณได้รับข้อผิดพลาดในระหว่างการซิงโครไนซ์เช่น "วัตถุที่ซิงโครไนซ์กับ ProxyAddress หรือ UserPrincipalName ที่มีอยู่แล้วในไดเรกทอรีของคุณ" ให้ดูที่[ข้อผิดพลาดการซิงค์แอตทริบิวต์ของการวินิจฉัยและ remediate ซ้ำ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)</span><span class="sxs-lookup"><span data-stu-id="e08dc-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="e08dc-104">นอกจากนี้ให้พิจารณาการเปิดใช้งานแอตทริบิวต์ที่ซ้ำกัน</span><span class="sxs-lookup"><span data-stu-id="e08dc-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="e08dc-105">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ซิงโครไนซ์ข้อมูลประจำตัวและแอตทริบิวต์ที่ซ้ำกันมีความยืดหยุ่น](https://aka.ms/duplicateattributeresiliency)</span><span class="sxs-lookup"><span data-stu-id="e08dc-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>