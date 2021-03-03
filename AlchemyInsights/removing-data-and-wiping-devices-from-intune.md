---
title: การลบข้อมูลและการลบอุปกรณ์จาก Intun1
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416332"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="cfb1b-102">การลบข้อมูลและการลบอุปกรณ์จาก Intun1</span><span class="sxs-lookup"><span data-stu-id="cfb1b-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="cfb1b-103">การเลิกใช้อุปกรณ์และการล้างอุปกรณ์การล้างอุปกรณ์สามารถใช้เพื่อเอาข้อมูลบริษัทที่จัดการโดย Intun> ออก หรือเพื่อรีเซ็ตเป็นค่าจากโรงงาน และส่งคืนอุปกรณ์เป็นการตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="cfb1b-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="cfb1b-104">ลงชื่อเข้าใช้การจัดการอุปกรณ์ Microsoft 365 แล้วไปที่  >  **อุปกรณ์ทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="cfb1b-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="cfb1b-105">เลือกอุปกรณ์ที่คุณต้องการลบข้อมูล</span><span class="sxs-lookup"><span data-stu-id="cfb1b-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="cfb1b-106">เลือกชนิดของการลบข้อมูลระยะไกลที่คุณต้องการลบ</span><span class="sxs-lookup"><span data-stu-id="cfb1b-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="cfb1b-107">การเลิกใช้จะลบข้อมูลขององค์กรเท่านั้น ในขณะที่การลบข้อมูลทั้งหมดจะคืนค่าอุปกรณ์กลับเป็นการตั้งค่าจากโรงงาน</span><span class="sxs-lookup"><span data-stu-id="cfb1b-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="cfb1b-108">เลือกใช่ เพื่อยืนยัน</span><span class="sxs-lookup"><span data-stu-id="cfb1b-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="cfb1b-109">จนกว่าการลบข้อมูลจะเสร็จสิ้น สถานะการกระบงของอุปกรณ์จะแสดง *เป็น เกษียณที่ค้าง* อยู่</span><span class="sxs-lookup"><span data-stu-id="cfb1b-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="cfb1b-110">หลังจากการแอคชันเสร็จสมบูรณ์ คุณจะไม่เห็นอุปกรณ์เคลื่อนที่ในรายการของอุปกรณ์ที่มีการจัดการอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="cfb1b-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="cfb1b-111">ไม่สามารถเอาข้อมูลบริษัทออกจากอุปกรณ์ที่เข้าร่วมไปยัง Azure AD ได้</span><span class="sxs-lookup"><span data-stu-id="cfb1b-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="cfb1b-112">For full details of the effect of the Retired and Wipe actions, including what is retained and what is deleted, see following documentation:</span><span class="sxs-lookup"><span data-stu-id="cfb1b-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="cfb1b-113">[ลบอุปกรณ์ออกโดยใช้การลบข้อมูล เลิกใช้ หรือยกเลิกการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="cfb1b-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="cfb1b-114">วิธีการลบข้อมูลขององค์กรจากแอป Intun1 ที่มีการจัดการเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="cfb1b-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="cfb1b-115">[ลบข้อมูลทั้งหมดจากอุปกรณ์ macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)</span><span class="sxs-lookup"><span data-stu-id="cfb1b-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>