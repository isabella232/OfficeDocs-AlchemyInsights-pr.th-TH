---
title: ข้อผิดพลาดการลงชื่อเข้าใช้ของ Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358367"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="e3b83-102">ข้อผิดพลาดการลงชื่อเข้าใช้ของ Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="e3b83-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="e3b83-103">เมื่อลงชื่อเข้าใช้ Microsoft Teams คุณอาจได้รับข้อผิดพลาด: ขออภัย**แต่เรากําลังมีปัญหาในการลงชื่อเข้าใช้ AADSTS9000411: การร้องขอไม่ได้รับการจัดรูปแบบอย่างถูกต้อง พารามิเตอร์ "login_hint" ซ้ํากัน**</span><span class="sxs-lookup"><span data-stu-id="e3b83-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="e3b83-104">เมื่อต้องการแก้ไขปัญหานี้ โปรดตรวจสอบให้แน่ใจว่าไคลเอนต์ Microsoft Teams ของคุณได้รับการปรับปรุงแล้ว</span><span class="sxs-lookup"><span data-stu-id="e3b83-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="e3b83-105">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการปรับปรุงไคลเอ็นต์ของคุณ ให้ดูที่ การปรับปรุง[Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="e3b83-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="e3b83-106">ถ้าคุณไม่สามารถปรับปรุงไคลเอนต์ของคุณด้วยเหตุผลบางอย่าง</span><span class="sxs-lookup"><span data-stu-id="e3b83-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="e3b83-107">อย่างไรก็ตาม หากคุณยังคงมีปัญหาหลังจากออกจากระบบ/ล็อกออน ออกจาก Teams และโปรดล้างแคชไคลเอ็นต์ของคุณโดยทําดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e3b83-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="e3b83-108">ปิด Microsoft ทีม</span><span class="sxs-lookup"><span data-stu-id="e3b83-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="e3b83-109">ไปที่: %appdata%\microsoft\ทีม และลบไฟล์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e3b83-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="e3b83-110">เปิดทีม Microsoft อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="e3b83-110">Reopen Microsoft Teams.</span></span>
