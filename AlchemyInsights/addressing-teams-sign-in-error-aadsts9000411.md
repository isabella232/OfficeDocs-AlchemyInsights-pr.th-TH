---
title: แก้ไขข้อผิดพลาดการลงชื่อเข้าใช้ Teams AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822006"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="b9065-102">แก้ไขข้อผิดพลาดการลงชื่อเข้าใช้ Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="b9065-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="b9065-103">เมื่อลงชื่อเข้าใช้ Microsoft Teams คุณอาจได้รับข้อผิดพลาด: ขออภัย เราพบปัญหาในการลงชื่อเข้าใช้ **AADSTS9000411: ไม่สามารถจัดรูปแบบการร้องขอได้อย่างถูกต้อง พารามิเตอร์ "login_hint" จะถูกคัดลอก**</span><span class="sxs-lookup"><span data-stu-id="b9065-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="b9065-104">เมื่อต้องการแก้ไขปัญหานี้ โปรดตรวจสอบให้แน่ใจว่าลูกค้า Microsoft Teams ของคุณได้รับการอัปเดตแล้ว</span><span class="sxs-lookup"><span data-stu-id="b9065-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="b9065-105">ดูข้อมูลเพิ่มเติมเกี่ยวกับการอัปเดตลูกค้าของคุณที่[อัปเดต Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="b9065-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="b9065-106">ถ้าคุณไม่สามารถอัปเดตไคลเอ็นต์ของคุณด้วยเหตุผลบางอย่าง การบันทึกออกจากไคลเอ็นต์จะล้างข้อมูลที่แคชส่วนใหญ่</span><span class="sxs-lookup"><span data-stu-id="b9065-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="b9065-107">อย่างไรก็ตาม ถ้าคุณยังคงมีปัญหาหลังจากออกจาก Logoff/logon ให้ออกจาก Teams และโปรดล้างแคชไคลเอ็นต์ของคุณโดยวิธีการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b9065-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="b9065-108">ปิด Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b9065-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="b9065-109">ไปที่: %appdata%\microsoft\teams แล้วลบไฟล์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="b9065-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="b9065-110">เปิด Microsoft Teams อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b9065-110">Reopen Microsoft Teams.</span></span>
