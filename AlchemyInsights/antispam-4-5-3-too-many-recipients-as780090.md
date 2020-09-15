---
title: ๑๐๔๙แอนติสแปม4.5.3 ผู้รับจำนวนมากเกินไป (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: deb57e6e872ce5769a339c7d130a63a8e90ab4c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717812"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="661af-102">4.5.3 ผู้รับจำนวนมากเกินไป (AS780090)</span><span class="sxs-lookup"><span data-stu-id="661af-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="661af-103">ข้อผิดพลาดนี้จะเกิดขึ้นเมื่อระดับเสียงของการรับส่งข้อมูลอีเมลจากที่อยู่ IP ของแหล่งข้อมูลเกินขีดจำกัดที่ยึดตามชื่อเสียง (หรือการขาดชื่อเสียง) ของที่อยู่ IP ของแหล่งข้อมูล</span><span class="sxs-lookup"><span data-stu-id="661af-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="661af-104">การบล็อกอีเมลจากที่อยู่ IP ของแหล่งข้อมูลจะหมดอายุภายในหนึ่งชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="661af-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="661af-105">ถ้าที่อยู่ IP ของแหล่งที่มาเป็นเซิร์ฟเวอร์อีเมลในสถานที่ที่เป็นของคุณให้ตรวจสอบการกำหนดค่าของตัวเชื่อมต่อลำดับจดหมาย</span><span class="sxs-lookup"><span data-stu-id="661af-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="661af-106">ถ้าลักษณะการทำงานยังคงเป็นเวลามากกว่าหนึ่งชั่วโมงให้ติดต่อฝ่ายสนับสนุนเพื่อร้องขอข้อยกเว้นสำหรับที่อยู่ IP ของแหล่งข้อมูล</span><span class="sxs-lookup"><span data-stu-id="661af-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
