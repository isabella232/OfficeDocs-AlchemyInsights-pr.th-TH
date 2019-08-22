---
title: 902 (ข้อผิดพลาดเนื่องจากวัตถุที่ซ้ำกัน)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507434"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="5e536-102">ข้อผิดพลาดในการซิงค์ได้เนื่องจากวัตถุที่ซ้ำกัน</span><span class="sxs-lookup"><span data-stu-id="5e536-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="5e536-103">คุณอาจได้รับข้อความแสดงข้อผิดพลาดต่อไปนี้เมื่อเสร็จสิ้นการซิงโครไนส์ของไดเรกทอรีใน Office 365:</span><span class="sxs-lookup"><span data-stu-id="5e536-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="5e536-104">ไม่สามารถปรับปรุงวัตถุนี้ในบริการออนไลน์ของ Microsoft ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในไดเรกทอรีภายในเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="5e536-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="5e536-105">วัตถุทำข้อมูลให้ตรงกับที่อยู่พร็อกซีเดียวกันอยู่แล้วในไดเรกทอรีการบริการแบบออนไลน์ของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="5e536-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="5e536-106">ไม่สามารถปรับปรุงวัตถุนี้ได้เนื่องจากแอตทริบิวต์ต่อไปนี้ที่เกี่ยวข้องกับวัตถุนี้มีค่าที่มีอยู่แล้วอาจเกี่ยวข้องกับวัตถุอื่นในบริการไดเรกทอรีภายในเครื่องของคุณ: UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e536-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="5e536-107">เมื่อต้องการระบุ และแก้ไขปัญหา ดาวน์โหลด และเรียกใช้[เครื่องมือด้านข้อผิดพลาดของ DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832)</span><span class="sxs-lookup"><span data-stu-id="5e536-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="5e536-108">สำหรับข้อมูลเพิ่มเติม ให้ดู[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="5e536-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
