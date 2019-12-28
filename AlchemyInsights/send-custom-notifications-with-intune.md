---
title: ส่งการแจ้งเตือนที่กำหนดเองด้วย Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886876"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a51b6-102">วิธีการส่งการแจ้งเตือนที่กำหนดเองไปยังผู้ใช้ของอุปกรณ์ iOS และ Android ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="a51b6-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a51b6-103">การแจ้งเตือนแบบกำหนดเองสำหรับ Intune จะถูกประมวลผลโดยแอพลิเคชันพอร์ทัลของบริษัทบนอุปกรณ์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a51b6-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a51b6-104">การตรวจสอบแล้วสร้างการแจ้งเตือนผลักดันบนอุปกรณ์ที่</span><span class="sxs-lookup"><span data-stu-id="a51b6-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a51b6-105">ต่อไปนี้เป็นข้อกำหนดเบื้องต้นของอุปกรณ์เพื่อสนับสนุนการรับการแจ้งเตือนที่กำหนดเองและสำหรับแอปเพื่อสร้างการแจ้งเตือนแบบพุช:</span><span class="sxs-lookup"><span data-stu-id="a51b6-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a51b6-106">อุปกรณ์ต้องมีการติดตั้งแอพ Portal ของบริษัท</span><span class="sxs-lookup"><span data-stu-id="a51b6-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a51b6-107">อุปกรณ์ต้องอนุญาตให้แอพลิเคชันพอร์ทัลของบริษัทส่งการแจ้งเตือนแบบพุช</span><span class="sxs-lookup"><span data-stu-id="a51b6-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a51b6-108">เมื่อมีการติดตั้งหรือปรับปรุงแอปพลิเคชันจะพร้อมท์ให้ผู้ใช้อนุญาตการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="a51b6-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a51b6-109">อุปกรณ์ Android จะต้องมีการติดตั้งบริการ Google Play</span><span class="sxs-lookup"><span data-stu-id="a51b6-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a51b6-110">อุปกรณ์ต้องลงทะเบียนกับ Intune</span><span class="sxs-lookup"><span data-stu-id="a51b6-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a51b6-111">สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการส่งข้อความให้ดูที่[เอกสารคุณลักษณะ](https://docs.microsoft.com/intune/custom-notifications)</span><span class="sxs-lookup"><span data-stu-id="a51b6-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
