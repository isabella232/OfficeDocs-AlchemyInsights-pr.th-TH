---
title: เหตุใดจึงไม่มีการปรับใช้การอัปเดตซอฟต์แวร์
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003773"
- "6717"
ms.openlocfilehash: 8e539260e1d99f18bf9bec32ae244c94aeebddbc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51805705"
---
# <a name="why-software-updates-are-not-being-deployed"></a><span data-ttu-id="d25fd-102">เหตุใดจึงไม่มีการปรับใช้การอัปเดตซอฟต์แวร์</span><span class="sxs-lookup"><span data-stu-id="d25fd-102">Why software updates are not being deployed?</span></span>

<span data-ttu-id="d25fd-103">ตรวจสอบต่อไปนี้ ถ้าคุณกําหนดค่าการอัปเดตซอฟต์แวร์ผ่านวงรอบการอัปเดต Windows 10 แต่การอัปเดตจะไม่ถูกปรับใช้:</span><span class="sxs-lookup"><span data-stu-id="d25fd-103">Review the following if you configured software updates through a Windows 10 update ring but the updates are not being deployed:</span></span>  

- <span data-ttu-id="d25fd-104">พิจารณาเปลี่ยนการให้บริการ Windows จาก  **ช่องทางรายครึ่ง**  ปีเป็นประเภทการเผยแพร่ที่เข้มงวดและบ่อยขึ้น</span><span class="sxs-lookup"><span data-stu-id="d25fd-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type</span></span>  
- <span data-ttu-id="d25fd-105">ตรวจสอบช่วงการเลื่อนเวลา **การอัปเดตคุณภาพ\*\*\*\*และการอัปเดต** ฟีเจอร์</span><span class="sxs-lookup"><span data-stu-id="d25fd-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="d25fd-106">ช่วงเวลาการยืดเวลาอาจส่งผลให้การอัปเดตล่าช้าเป็นเวลา 180 วัน</span><span class="sxs-lookup"><span data-stu-id="d25fd-106">The deferral period could lead to delay in updates for up 180 days.</span></span>
