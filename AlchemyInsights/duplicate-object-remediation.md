---
title: "1314"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1314"
- "1300024"
ms.assetid: b8543b7e-fd00-4b3c-be68-a1758b8caf78
ms.openlocfilehash: 138ba305b872e8c0508ba673fb59324672d14997
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703986"
---
# <a name="duplicate-object-synchronization-errors"></a><span data-ttu-id="e522d-102">ข้อผิดพลาดการทําข้อมูลออบเจ็กต์ซ้ํา</span><span class="sxs-lookup"><span data-stu-id="e522d-102">Duplicate object synchronization errors</span></span>

<span data-ttu-id="e522d-103">ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้อย่างใดอย่างหนึ่งในระหว่างการซิงโครไนส์:</span><span class="sxs-lookup"><span data-stu-id="e522d-103">If you receive one of the following errors during a synchronization:</span></span>

- <span data-ttu-id="e522d-104">มีวัตถุที่ซิงโครไนส์กับที่อยู่พร็อกซีเดียวกันอยู่แล้วในไดเรกทอรีบริการออนไลน์ของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="e522d-104">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="e522d-105">ข้อความที่คล้ายกันสําหรับชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e522d-105">A similar message for UserPrincipalName.</span></span>

<span data-ttu-id="e522d-106">ใช้การวินิจฉัยความสมบูรณ์ AADConnect ใหม่เพื่อแก้ไขข้อผิดพลาดของวัตถุที่ซ้ํากัน</span><span class="sxs-lookup"><span data-stu-id="e522d-106">Use the new AADConnect Health diagnostic to resolve duplicate object errors.</span></span> <span data-ttu-id="e522d-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วินิจฉัยและแก้ไขข้อผิดพลาดการซิงค์แอตทริบิวต์ที่ซ้ํากัน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)</span><span class="sxs-lookup"><span data-stu-id="e522d-107">For more information, see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>
