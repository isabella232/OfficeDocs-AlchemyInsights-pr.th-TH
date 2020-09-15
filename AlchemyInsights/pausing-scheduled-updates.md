---
title: การอัปเดตที่จัดกำหนดการชั่วคราว
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721574"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="3d5d0-102">การอัปเดตที่จัดกำหนดการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="3d5d0-102">Pausing scheduled updates</span></span>

<span data-ttu-id="3d5d0-103">เมื่อมีการออกคำสั่งหยุดชั่วคราวอุปกรณ์จะไม่ประมวลผลคำสั่งจนกว่าพวกเขาจะเช็คอินไปยัง Intune ในครั้งถัดไป</span><span class="sxs-lookup"><span data-stu-id="3d5d0-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="3d5d0-104">เนื่องจากการทำเช่นนี้อุปกรณ์ของคุณอาจมีสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="3d5d0-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="3d5d0-105">ติดตั้งการอัปเดตที่จัดกำหนดการไว้ก่อนที่จะเช็คอิน</span><span class="sxs-lookup"><span data-stu-id="3d5d0-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="3d5d0-106">ถูกปิดใช้งานเมื่อคุณออกคำสั่งหยุดชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="3d5d0-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="3d5d0-107">ในกรณีนี้เมื่ออุปกรณ์เปิดอยู่แล้วอุปกรณ์เหล่านั้นอาจได้รับการดาวน์โหลดและติดตั้งการอัปเดตที่จัดกำหนดการไว้ก่อนที่จะเช็คอิน</span><span class="sxs-lookup"><span data-stu-id="3d5d0-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>