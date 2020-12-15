---
title: ลงชื่อเข้าใช้ Microsoft Edge ด้วยตนเอง
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678847"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="b5d8e-102">ลงชื่อเข้าใช้ Microsoft Edge ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="b5d8e-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="b5d8e-103">ถ้าผู้ใช้ไม่ได้ลงชื่อเข้าใช้โดยอัตโนมัติในระหว่างประสบการณ์การใช้งานครั้งแรกผู้ใช้สามารถลงชื่อเข้าใช้ด้วยตนเองผ่านการตั้งค่าของเบราว์เซอร์หรือการลอยตัวของข้อมูลประจำตัว</span><span class="sxs-lookup"><span data-stu-id="b5d8e-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="b5d8e-104">เมื่อต้องการจัดการการลงชื่อเข้าใช้ให้ใช้นโยบายต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b5d8e-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="b5d8e-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -เพื่อให้แน่ใจว่าผู้ใช้มีโปรไฟล์ที่ทำงานใน Microsoft Edge เสมอ</span><span class="sxs-lookup"><span data-stu-id="b5d8e-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="b5d8e-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -เมื่อต้องการจำกัดการลงชื่อเข้าใช้ในชุดของบัญชีผู้ใช้ที่เชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="b5d8e-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="b5d8e-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -เมื่อต้องการปิดใช้งานการลงชื่อเข้าใช้หรือการบังคับให้ผู้ใช้ลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="b5d8e-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

