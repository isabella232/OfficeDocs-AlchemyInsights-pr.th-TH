---
title: เหตุใดการอัปเดตซอฟต์แวร์จึงไม่ถูกจัดวาง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003773"
- "6717"
ms.openlocfilehash: 2e7156f994d27f46cec6dcc3c8680b55ebfe3ec2
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461980"
---
# <a name="why-software-updates-are-not-being-deployed"></a><span data-ttu-id="5b2a0-102">เหตุใดการอัปเดตซอฟต์แวร์จึงไม่ถูกจัดวาง</span><span class="sxs-lookup"><span data-stu-id="5b2a0-102">Why software updates are not being deployed?</span></span>

<span data-ttu-id="5b2a0-103">ตรวจทานสิ่งต่อไปนี้ถ้าคุณได้กำหนดค่าการอัปเดตซอฟต์แวร์ผ่านทางการอัปเดต Windows 10 แต่การอัปเดตจะไม่ถูกปรับใช้:</span><span class="sxs-lookup"><span data-stu-id="5b2a0-103">Review the following if you configured software updates through a Windows 10 update ring but the updates are not being deployed:</span></span>  

- <span data-ttu-id="5b2a0-104">พิจารณาเปลี่ยนการให้บริการของ Windows จากชนิดการวางจำหน่ายแบบ  **ครึ่งรายครึ่งปี**  เป็นชนิดที่เข้มงวดมากขึ้นเป็นชนิดการวางจำหน่ายบ่อย</span><span class="sxs-lookup"><span data-stu-id="5b2a0-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type</span></span>  
- <span data-ttu-id="5b2a0-105">ตรวจสอบการอัปเด deferral สำหรับการอัปเด**ตที่มีคุณภาพ**และการ**อัปเดตของฟีเจอร์**</span><span class="sxs-lookup"><span data-stu-id="5b2a0-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="5b2a0-106">ช่วงเวลา deferral สามารถนำไปสู่การหน่วงเวลาในการอัปเดตสำหรับวันที่๑๘๐ได้</span><span class="sxs-lookup"><span data-stu-id="5b2a0-106">The deferral period could lead to delay in updates for up 180 days.</span></span>
