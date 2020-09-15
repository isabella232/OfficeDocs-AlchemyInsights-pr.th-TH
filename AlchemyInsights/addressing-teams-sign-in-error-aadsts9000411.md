---
title: การกำหนดความผิดพลาดในการลงชื่อเข้าใช้ในทีม AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687057"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="44d2c-102">การกำหนดความผิดพลาดในการลงชื่อเข้าใช้ในทีม AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="44d2c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="44d2c-103">เมื่อคุณลงชื่อเข้าใช้ Microsoft team คุณอาจได้รับข้อผิดพลาด: **ขออภัยแต่เรากำลังมีปัญหาเกี่ยวกับการลงชื่อเข้าใช้คุณใน AADSTS9000411: การร้องขอจะไม่ถูกจัดรูปแบบอย่างถูกต้อง พารามิเตอร์ "login_hint" จะซ้ำกัน**</span><span class="sxs-lookup"><span data-stu-id="44d2c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="44d2c-104">เมื่อต้องการแก้ปัญหานี้โปรดตรวจสอบให้แน่ใจว่าไคลเอ็นต์ Microsoft team ของคุณได้รับการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="44d2c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="44d2c-105">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการอัปเดตลูกค้าของคุณให้ดูที่[อัปเดต Microsoft ทีม](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="44d2c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="44d2c-106">ถ้าคุณไม่สามารถอัปเดตไคลเอ็นต์ของคุณได้ด้วยเหตุผลบางประการการออกจากระบบไคลเอ็นต์จะล้างข้อมูลที่แคชไว้ที่สุด</span><span class="sxs-lookup"><span data-stu-id="44d2c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="44d2c-107">อย่างไรก็ตามถ้าคุณยังคงมีปัญหาหลังจากออกจากระบบ/เข้าสู่ระบบออกจากทีมและโปรดล้างแคชของไคลเอ็นต์ของคุณโดยทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="44d2c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="44d2c-108">ปิดทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="44d2c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="44d2c-109">ไปที่:%appdata%\microsoft\teams และลบไฟล์ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="44d2c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="44d2c-110">เปิดทีม Microsoft อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="44d2c-110">Reopen Microsoft Teams.</span></span>
