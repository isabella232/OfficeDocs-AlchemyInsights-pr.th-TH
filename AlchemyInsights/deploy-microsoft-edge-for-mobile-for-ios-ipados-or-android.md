---
title: ปรับใช้ Microsoft Edge สำหรับอุปกรณ์เคลื่อนที่สำหรับ iOS/iPadOS หรือ Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679946"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="e097a-102">ปรับใช้ Microsoft Edge สำหรับอุปกรณ์เคลื่อนที่สำหรับ iOS/iPadOS หรือ Android</span><span class="sxs-lookup"><span data-stu-id="e097a-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="e097a-103">สถานการณ์สมมติที่แนะนำด้านล่างนี้จะช่วยให้คุณสามารถกำหนด Microsoft Edge ให้กับผู้ใช้อุปกรณ์ iOS, iPadOS และ Android</span><span class="sxs-lookup"><span data-stu-id="e097a-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="e097a-104">หลังจากที่คุณทำตามขั้นตอนเหล่านี้แล้วนโยบาย Microsoft Intune จะเปิดใช้งานฟีเจอร์ต่อไปนี้ของ Microsoft Edge for business:</span><span class="sxs-lookup"><span data-stu-id="e097a-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="e097a-105">เอกลักษณ์คู่</span><span class="sxs-lookup"><span data-stu-id="e097a-105">Dual identity</span></span>
- <span data-ttu-id="e097a-106">การรวมเข้ากับนโยบายการป้องกันแอป Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e097a-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="e097a-107">การรวมกับพร็อกซีแอปพลิเคชัน active Directory ของ Azure</span><span class="sxs-lookup"><span data-stu-id="e097a-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="e097a-108">รายการโปรดที่มีการจัดการและทางลัดโฮมเพจ</span><span class="sxs-lookup"><span data-stu-id="e097a-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="e097a-109">ถ้าคุณบล็อกผู้ใช้จากการลงทะเบียนอุปกรณ์เคลื่อนที่สถานการณ์สมมติที่แนะนำนี้จะไม่ทำงานและผู้ใช้จะต้องติดตั้ง Microsoft Edge ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="e097a-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="e097a-110">เมื่อต้องการปรับใช้ Microsoft Edge สำหรับอุปกรณ์เคลื่อนที่สำหรับ iOS/iPadOS หรือ Android ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="e097a-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="e097a-111">เบื้อง</span><span class="sxs-lookup"><span data-stu-id="e097a-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="e097a-112">บทนำสู่</span><span class="sxs-lookup"><span data-stu-id="e097a-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="e097a-113">พื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="e097a-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="e097a-114">กำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="e097a-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="e097a-115">กำหนด</span><span class="sxs-lookup"><span data-stu-id="e097a-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="e097a-116">รีวิวและการสร้าง</span><span class="sxs-lookup"><span data-stu-id="e097a-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
