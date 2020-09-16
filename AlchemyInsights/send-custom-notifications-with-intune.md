---
title: ส่งการแจ้งเตือนแบบกำหนดเองด้วย Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720665"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="dc871-102">วิธีการส่งการแจ้งเตือนแบบกำหนดเองไปยังผู้ใช้ของอุปกรณ์ iOS และ Android ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="dc871-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="dc871-103">การแจ้งเตือนแบบกำหนดเองสำหรับ Intune จะถูกประมวลผลโดยแอปพอร์ทัลของบริษัทบนอุปกรณ์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="dc871-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="dc871-104">แอปจะสร้างการแจ้งเตือนแบบพุชบนอุปกรณ์นั้น</span><span class="sxs-lookup"><span data-stu-id="dc871-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="dc871-105">ต่อไปนี้คือข้อกำหนดเบื้องต้นของอุปกรณ์เพื่อสนับสนุนการรับการแจ้งเตือนแบบกำหนดเองและสำหรับแอปเพื่อสร้างการแจ้งเตือนแบบพุช:</span><span class="sxs-lookup"><span data-stu-id="dc871-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="dc871-106">อุปกรณ์จำเป็นต้องติดตั้งแอปพอร์ทัลบริษัท</span><span class="sxs-lookup"><span data-stu-id="dc871-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="dc871-107">อุปกรณ์ต้องอนุญาตให้แอป Portal ของบริษัทส่งการแจ้งเตือนแบบพุช</span><span class="sxs-lookup"><span data-stu-id="dc871-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="dc871-108">เมื่อแอปได้รับการติดตั้งหรืออัปเดตโปรแกรมจะพร้อมท์ให้ผู้ใช้อนุญาตการแจ้งให้ทราบ</span><span class="sxs-lookup"><span data-stu-id="dc871-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="dc871-109">อุปกรณ์ Android ต้องมีการติดตั้งบริการ Google Play</span><span class="sxs-lookup"><span data-stu-id="dc871-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="dc871-110">อุปกรณ์ต้องลงทะเบียนด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="dc871-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="dc871-111">สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการส่งข้อความให้ดูที่[เอกสารประกอบของฟีเจอร์](https://docs.microsoft.com/intune/custom-notifications)</span><span class="sxs-lookup"><span data-stu-id="dc871-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
