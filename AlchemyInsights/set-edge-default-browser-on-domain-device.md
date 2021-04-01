---
title: ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้นบนอุปกรณ์ที่เข้าร่วมในโดเมน
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
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491876"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="f7eee-102">ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้นบนอุปกรณ์ที่เข้าร่วมในโดเมน</span><span class="sxs-lookup"><span data-stu-id="f7eee-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="f7eee-103">ตั้งค่า Microsoft Edge เป็นเบราว์เซอร์เริ่มต้น:</span><span class="sxs-lookup"><span data-stu-id="f7eee-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="f7eee-104">[สร้างไฟล์การกําหนดค่าความสัมพันธ์เริ่มต้น](https://go.microsoft.com/fwlink/?linkid=2132437) และจัดเก็บไว้ภายในเครื่องหรือบนเครือข่ายที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="f7eee-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="f7eee-105">เปิดตัวแก้ไขนโยบายกลุ่ม แล้วไปที่การกําหนด **ค่าคอมพิวเตอร์เทมเพลต**  >  **การดูแลระบบ**  >  **File**  >  **Explorer คอมโพเนนต์** ของ Windows</span><span class="sxs-lookup"><span data-stu-id="f7eee-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="f7eee-106">เลือก **ตั้งค่าไฟล์การกําหนดค่าความสัมพันธ์** เริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f7eee-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="f7eee-107">**เลือกการตั้งค่า** นโยบาย **จากนั้นเลือก** เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f7eee-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="f7eee-108">ภายใต้ **ตัวเลือก** ให้ใส่ที่ตั้งของไฟล์การกําหนดค่าความสัมพันธ์เริ่มต้นของคุณ **แล้วเลือก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="f7eee-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
