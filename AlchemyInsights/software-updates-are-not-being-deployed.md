---
title: การปรับปรุงซอฟต์แวร์จะไม่ถูกปรับใช้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1125"
- "6700007"
ms.openlocfilehash: 418f457700f02881df30e6f650a60101192aa538
ms.sourcegitcommit: 3fa780811984400c525d66edf46a3196f6290df0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/23/2020
ms.locfileid: "45424108"
---
# <a name="software-updates-are-not-being-deployed"></a><span data-ttu-id="fa15b-102">การปรับปรุงซอฟต์แวร์จะไม่ถูกปรับใช้</span><span class="sxs-lookup"><span data-stu-id="fa15b-102">Software updates are not being deployed</span></span>

<span data-ttu-id="fa15b-103">ถ้าคุณกําหนดค่าการปรับปรุงซอฟต์แวร์ผ่านวงแหวนการปรับปรุง Windows 10 แต่การปรับปรุงจะไม่ถูกปรับใช้ ให้ลองทําดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fa15b-103">If you configured software updates through a Windows 10 update ring, but the updates are not being deployed, try the following:</span></span>  

- <span data-ttu-id="fa15b-104">พิจารณาเปลี่ยนบริการของ Windows จากประเภทการเผยแพร่**แบบกึ่งรายปี**เป็นประเภทการนําออกใช้ที่เข้มงวดขึ้น</span><span class="sxs-lookup"><span data-stu-id="fa15b-104">Consider changing Windows servicing from a  **Semi-Annual Channel**  release type to a stricter, more frequent release type.</span></span>
- <span data-ttu-id="fa15b-105">ตรวจสอบรอบระยะเวลารอการตัดบัญชีสําหรับ**การปรับปรุงคุณภาพ**และ**การปรับปรุงคุณลักษณะ**</span><span class="sxs-lookup"><span data-stu-id="fa15b-105">Check the deferral period for  **Quality update**  and  **Feature update**.</span></span> <span data-ttu-id="fa15b-106">ระยะเวลารอการตัดบัญชีอาจนําไปสู่ความล่าช้าในการปรับปรุงได้ถึง 180 วัน</span><span class="sxs-lookup"><span data-stu-id="fa15b-106">A deferral period could lead to a delay in updates for up to 180 days.</span></span>