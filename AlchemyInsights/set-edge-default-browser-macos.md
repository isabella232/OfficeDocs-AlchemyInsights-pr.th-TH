---
title: ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้นบนอุปกรณ์ macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491817"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="1e245-102">ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้นบนอุปกรณ์ macOS</span><span class="sxs-lookup"><span data-stu-id="1e245-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="1e245-103">ใช้หนึ่งในสองวิธีต่อไปนี้เพื่อตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้น:</span><span class="sxs-lookup"><span data-stu-id="1e245-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="1e245-104">วิธีที่ 1: แฟลชอุปกรณ์ด้วยรูปภาพของ macOS ที่ Microsoft Edge ถูกตั้งค่าเป็นเบราว์เซอร์เริ่มต้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="1e245-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="1e245-105">วิธีที่ 2: ตั้งค่านโยบาย DefaultBrowserSettingEnabled เพื่อพร้อมท์ผู้ใช้ให้ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="1e245-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="1e245-106">ทั้งสองวิธีอนุญาตให้ผู้ใช้เปลี่ยนเบราว์เซอร์เริ่มต้นได้</span><span class="sxs-lookup"><span data-stu-id="1e245-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="1e245-107">ด้วยเหตุผลนี้ เราขอแนะนนะให้คุณปรับใช้นโยบาย DefaultBrowserSettingEnabled แม้ว่าคุณจะใช้วิธีที่ 1</span><span class="sxs-lookup"><span data-stu-id="1e245-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="1e245-108">ถ้าผู้ใช้เปลี่ยนเบราว์เซอร์เริ่มต้นหลังจากปรับใช้นโยบาย นโยบายจะพร้อมท์ให้ผู้ใช้ตั้งค่าเบราว์เซอร์เริ่มต้นกลับไปยัง Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1e245-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
