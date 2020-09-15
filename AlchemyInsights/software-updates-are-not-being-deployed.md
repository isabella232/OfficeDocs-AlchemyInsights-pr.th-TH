---
title: การอัปเดตซอฟต์แวร์ไม่ถูกจัดวาง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1125"
- "6700007"
ms.openlocfilehash: d9a37e4c2d977083cf2ccbf6580159f92524f936
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665269"
---
# <a name="software-updates-are-not-being-deployed"></a><span data-ttu-id="b8d0c-102">การอัปเดตซอฟต์แวร์ไม่ถูกจัดวาง</span><span class="sxs-lookup"><span data-stu-id="b8d0c-102">Software updates are not being deployed</span></span>

<span data-ttu-id="b8d0c-103">ถ้าคุณได้กำหนดค่าการอัปเดตซอฟต์แวร์ผ่านทางการอัปเดต Windows 10 แล้วแต่การอัปเดตจะไม่ได้รับการปรับใช้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b8d0c-103">If you configured software updates through a Windows 10 update ring, but the updates are not being deployed, try the following:</span></span>  

- <span data-ttu-id="b8d0c-104">พิจารณาการเปลี่ยนการให้บริการของ Windows จากชนิดการวางจำหน่ายของ  **แชนเนลแบบครึ่งรายครึ่งปี**  เป็นชนิดที่เข้มงวดมากขึ้นเป็นรุ่นที่ใช้บ่อย</span><span class="sxs-lookup"><span data-stu-id="b8d0c-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type.</span></span>
- <span data-ttu-id="b8d0c-105">ตรวจสอบการอัปเด deferral สำหรับการอัปเด**ตที่มีคุณภาพ**และการ**อัปเดตของฟีเจอร์**</span><span class="sxs-lookup"><span data-stu-id="b8d0c-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="b8d0c-106">ช่วงเวลา deferral สามารถนำไปสู่การหน่วงเวลาในการอัปเดตได้ถึง๑๘๐วัน</span><span class="sxs-lookup"><span data-stu-id="b8d0c-106">A deferral period could lead to a delay in updates for up to 180 days.</span></span>