---
title: การลบข้อมูลและล้างข้อมูลอุปกรณ์จาก Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440464"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="f7656-102">การลบข้อมูลและล้างข้อมูลอุปกรณ์จาก Intun</span><span class="sxs-lookup"><span data-stu-id="f7656-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="f7656-103">อุปกรณ์เลิกใช้อุปกรณ์และล้างข้อมูลอุปกรณ์จากระยะไกลสามารถใช้เพื่อลบข้อมูลบริษัทที่จัดการโดย Intun หรือเพื่อดําเนินการรีเซ็ตเป็นค่าเริ่มต้นและส่งคืนอุปกรณ์กลับไปใช้การตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="f7656-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="f7656-104">ลงชื่อเข้าใช้การจัดการอุปกรณ์ Microsoft 365 และไปที่**Devices**  >  **อุปกรณ์ทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="f7656-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="f7656-105">เลือกอุปกรณ์ที่คุณต้องการล้างข้อมูล</span><span class="sxs-lookup"><span data-stu-id="f7656-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="f7656-106">เลือกชนิดของการลบข้อมูลระยะไกลที่คุณต้องการทํา</span><span class="sxs-lookup"><span data-stu-id="f7656-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="f7656-107">ออกจะลบเฉพาะข้อมูลขององค์กรในขณะที่ล้างข้อมูลทั้งหมดจะคืนค่าอุปกรณ์ไปยังการตั้งค่าจากโรงงาน</span><span class="sxs-lookup"><span data-stu-id="f7656-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="f7656-108">เลือก**ใช่**เพื่อยืนยัน</span><span class="sxs-lookup"><span data-stu-id="f7656-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="f7656-109">สถานะการดําเนินการของอุปกรณ์จะแสดงเป็น</span><span class="sxs-lookup"><span data-stu-id="f7656-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="f7656-110">หลังจากการดําเนินการเสร็จสิ้นแล้ว คุณจะไม่เห็นอุปกรณ์เคลื่อนที่ในรายการอุปกรณ์ที่มีการจัดการอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="f7656-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="f7656-111">**หมายเหตุ** ไม่สามารถเอาข้อมูลบริษัทออกจากอุปกรณ์ที่เข้าร่วมไปยัง Azure AD ได้</span><span class="sxs-lookup"><span data-stu-id="f7656-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="f7656-112">สําหรับรายละเอียดทั้งหมดของผลของการกระทําการเกษียณอายุและเช็ด รวมถึงสิ่งที่ถูกเก็บไว้ และสิ่งที่ถูกลบ โปรดดูที่[นําอุปกรณ์ออกโดยใช้การล้างข้อมูล](https://docs.microsoft.com/intune/devices-wipe)</span><span class="sxs-lookup"><span data-stu-id="f7656-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="f7656-113">หากต้องการลบข้อมูลทั้งหมดออกจากอุปกรณ์ macOS โปรดดู[ลบข้อมูลทั้งหมดออกจากอุปกรณ์ macOS](https://docs.microsoft.com/intune/device-erase)</span><span class="sxs-lookup"><span data-stu-id="f7656-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>