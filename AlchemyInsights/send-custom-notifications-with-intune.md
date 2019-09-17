---
title: ส่งการแจ้งเตือนที่กำหนดเองด้วย Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992331"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a72d5-102">วิธีการส่งการแจ้งเตือนที่กำหนดเองไปยังผู้ใช้ของอุปกรณ์ iOS และ Android ที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="a72d5-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a72d5-103">การแจ้งเตือนแบบกำหนดเองสำหรับ Intune จะถูกประมวลผลโดยแอพลิเคชันพอร์ทัลของบริษัทบนอุปกรณ์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a72d5-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a72d5-104">การตรวจสอบแล้วสร้างการแจ้งเตือนผลักดันบนอุปกรณ์ที่</span><span class="sxs-lookup"><span data-stu-id="a72d5-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a72d5-105">ต่อไปนี้เป็นข้อกำหนดเบื้องต้นของอุปกรณ์เพื่อสนับสนุนการรับการแจ้งเตือนที่กำหนดเองและสำหรับแอปเพื่อสร้างการแจ้งเตือนแบบพุช:</span><span class="sxs-lookup"><span data-stu-id="a72d5-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a72d5-106">อุปกรณ์ต้องมีการติดตั้งแอพ Portal ของบริษัท</span><span class="sxs-lookup"><span data-stu-id="a72d5-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a72d5-107">อุปกรณ์ต้องอนุญาตให้แอพลิเคชันพอร์ทัลของบริษัทส่งการแจ้งเตือนแบบพุช</span><span class="sxs-lookup"><span data-stu-id="a72d5-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a72d5-108">เมื่อมีการติดตั้งหรือปรับปรุงแอปพลิเคชันจะพร้อมท์ให้ผู้ใช้อนุญาตการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="a72d5-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a72d5-109">อุปกรณ์ Android จะต้องมีการติดตั้งบริการ Google Play</span><span class="sxs-lookup"><span data-stu-id="a72d5-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a72d5-110">อุปกรณ์ต้องลงทะเบียนกับ Intune</span><span class="sxs-lookup"><span data-stu-id="a72d5-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a72d5-111">สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการส่งข้อความให้ดูที่[เอกสารคุณลักษณะ](https://docs.microsoft.com/intune/custom-notifications)</span><span class="sxs-lookup"><span data-stu-id="a72d5-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
