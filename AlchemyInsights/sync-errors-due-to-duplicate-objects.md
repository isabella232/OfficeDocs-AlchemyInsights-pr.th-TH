---
title: ๙๐๒ (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ำกัน)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737360"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="2da43-102">ข้อผิดพลาดการซิงค์เนื่องจากวัตถุที่ซ้ำกัน</span><span class="sxs-lookup"><span data-stu-id="2da43-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="2da43-103">คุณอาจได้รับข้อความแสดงข้อผิดพลาดอย่างใดอย่างหนึ่งต่อไปนี้เมื่อซิงโครไนซ์ไดเรกทอรีเสร็จสิ้นใน Microsoft ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="2da43-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="2da43-104">ไม่สามารถปรับปรุงวัตถุนี้ในบริการ Microsoft Online ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเกี่ยวข้องกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="2da43-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="2da43-105">วัตถุที่ซิงโครไนซ์ที่มีที่อยู่พร็อกซีเดียวกันมีอยู่แล้วในไดเรกทอรี Microsoft Online Services ของคุณ</span><span class="sxs-lookup"><span data-stu-id="2da43-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="2da43-106">ไม่สามารถอัปเดอ็อบเจกต์นี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่อาจเกี่ยวข้องกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2da43-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="2da43-107">เมื่อต้องการระบุและแก้ไขปัญหาให้ดาวน์โหลดและเรียกใช้[เครื่องมือการแก้ไขข้อผิดพลาดของ IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832)</span><span class="sxs-lookup"><span data-stu-id="2da43-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="2da43-108">สำหรับข้อมูลเพิ่มเติมให้ดูที่[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="2da43-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
