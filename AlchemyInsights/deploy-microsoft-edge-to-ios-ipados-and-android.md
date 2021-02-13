---
title: ปรับใช้ Microsoft Edge กับ iOS, iPadOS และ Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194585"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="21389-102">ปรับใช้ Microsoft Edge กับ iOS, iPadOS และ Android</span><span class="sxs-lookup"><span data-stu-id="21389-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="21389-103">สถานการณ์ชี้แนะที่สรุปไว้ด้านล่างจะช่วยให้คุณกําหนด Microsoft Edge ให้กับผู้ใช้อุปกรณ์ iOS, iPadOS และ Android</span><span class="sxs-lookup"><span data-stu-id="21389-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="21389-104">ถ้าคุณบล็อกผู้ใช้จากการลงทะเบียนอุปกรณ์เคลื่อนที่ สถานการณ์สมมติตามแนวทางนี้จะไม่ใช้งาน และผู้ใช้จะต้องติดตั้ง Microsoft Edge ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="21389-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="21389-105">สถานการณ์ที่แนะนะจะเกี่ยวข้องกับขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="21389-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="21389-106">โปรแกรมเบื้องต้น</span><span class="sxs-lookup"><span data-stu-id="21389-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="21389-107">บทนํา</span><span class="sxs-lookup"><span data-stu-id="21389-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="21389-108">พื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="21389-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="21389-109">การกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="21389-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="21389-110">งานที่มอบหมาย</span><span class="sxs-lookup"><span data-stu-id="21389-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="21389-111">รีวิวและการสร้าง</span><span class="sxs-lookup"><span data-stu-id="21389-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="21389-112">หลังจากคุณปฏิบัติตามขั้นตอนในสถานการณ์ที่แนะนะแล้ว นโยบาย Microsoft Intuned จะเปิดใช้งานฟีเจอร์ต่อไปนี้ของ Microsoft Edge for Business:</span><span class="sxs-lookup"><span data-stu-id="21389-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="21389-113">ข้อมูลเฉพาะตัวคู่</span><span class="sxs-lookup"><span data-stu-id="21389-113">Dual identity</span></span>
- <span data-ttu-id="21389-114">การรวมกับนโยบายการป้องกันแอป Microsoft Intun1</span><span class="sxs-lookup"><span data-stu-id="21389-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="21389-115">การรวมกับพร็อกซีแอปพลิเคชัน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="21389-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="21389-116">ทางลัดรายการโปรดและโฮมเพจที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="21389-116">Managed favorites and home page shortcuts</span></span>
