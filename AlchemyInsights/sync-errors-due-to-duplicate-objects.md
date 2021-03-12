---
title: 902 (ข้อผิดพลาดในการซิงค์เนื่องจากวัตถุที่ซ้ากัน)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708081"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="2e95e-102">การซิงค์ข้อผิดพลาดเนื่องจากวัตถุที่คัดลอกกัน</span><span class="sxs-lookup"><span data-stu-id="2e95e-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="2e95e-103">คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้เมื่อการซิงโครไนซ์ไดเรกทอรีเสร็จสิ้นใน Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="2e95e-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="2e95e-104">ไม่สามารถอัปเดตวัตถุนี้ใน Microsoft Online Services ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณอยู่แล้ว</span><span class="sxs-lookup"><span data-stu-id="2e95e-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="2e95e-105">วัตถุที่ซิงโครไนซ์ที่มีที่อยู่พร็อกซีเดียวกันมีอยู่แล้วในไดเรกทอรี Microsoft Online Services ของคุณ</span><span class="sxs-lookup"><span data-stu-id="2e95e-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="2e95e-106">ไม่สามารถอัปเดตวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เชื่อมโยงกับวัตถุนี้มีค่าที่อาจเชื่อมโยงกับวัตถุอื่นในบริการไดเรกทอรีภายในของคุณอยู่แล้ว: UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e95e-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="2e95e-107">เมื่อต้องการระบุและแก้ไขปัญหา ให้ดาวน์โหลดและเรียกใช้เครื่องมือแก้ไขปัญหาข้อผิดพลาด[IdFix DirSync](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="2e95e-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="2e95e-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="2e95e-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
