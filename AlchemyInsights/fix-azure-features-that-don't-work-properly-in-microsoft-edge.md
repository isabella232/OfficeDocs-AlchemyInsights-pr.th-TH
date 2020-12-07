---
title: สิ่งที่ต้องทำถ้าฟีเจอร์ Azure ทำงานไม่ถูกต้องใน Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583780"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="a7f0b-102">สิ่งที่ต้องทำถ้าฟีเจอร์ Azure ทำงานไม่ถูกต้องใน Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a7f0b-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="a7f0b-103">Microsoft Edge ได้ [ทราบปัญหา](https://go.microsoft.com/fwlink/?linkid=2140608) ที่เกี่ยวข้องกับโซนความปลอดภัยและอาจส่งผลต่อวิธีการเข้าสู่ระบบของผู้ใช้ Azure ในศูนย์การจัดการ Windows</span><span class="sxs-lookup"><span data-stu-id="a7f0b-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="a7f0b-104">ถ้าคุณกำลังมีปัญหาในการใช้ฟีเจอร์ Azure กับ Microsoft Edge ให้ลองทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a7f0b-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="a7f0b-105">ในเมนู **เริ่ม** ให้ค้นหา **ตัวเลือกอินเทอร์เน็ต** แล้วเลือก</span><span class="sxs-lookup"><span data-stu-id="a7f0b-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="a7f0b-106">ในกล่องโต้ตอบ **คุณสมบัติของอินเทอร์เน็ต** ให้ไปที่แท็บ **ความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="a7f0b-107">เลือกโซน **ไซต์ที่เชื่อถือ** ได้แล้วเลือกปุ่ม **ไซต์**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="a7f0b-108">ในกล่องโต้ตอบ **ไซต์ที่เชื่อถือได้** ให้เพิ่ม URL ของเกตเวย์ของคุณเช่นเดียวกับ [https://login.microsoftonline.com](https://login.microsoftonline.com) และ [https://login.live.com](https://login.live.com) จากนั้นเลือก **ปิด**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="a7f0b-109">ในกล่องโต้ตอบ **คุณสมบัติของอินเทอร์เน็ต** ให้ไปที่แท็บ **ความเป็นส่วนตัว**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="a7f0b-110">ในส่วนตัว **บล็อก** ป็อปอัพให้เลือก **การตั้งค่า**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="a7f0b-111">ในกล่องโต้ตอบที่เปิดขึ้นให้เพิ่ม URL ของเกตเวย์ของคุณรวมถึง [https://login.microsoftonline.com](https://login.microsoftonline.com) และ [https://login.live.com](https://login.live.com) จากนั้นเลือก **ปิด**</span><span class="sxs-lookup"><span data-stu-id="a7f0b-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
