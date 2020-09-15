---
title: การเอาข้อมูลและการเช็ดอุปกรณ์ออกจาก Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701302"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="8a4a4-102">การเอาข้อมูลและการเช็ดอุปกรณ์ออกจาก Intune</span><span class="sxs-lookup"><span data-stu-id="8a4a4-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="8a4a4-103">อุปกรณ์ถอนการติดตั้งและลบการดำเนินการระยะไกลสามารถใช้เพื่อเอาข้อมูลบริษัทที่จัดการโดย Intune หรือดำเนินการตั้งค่าจากโรงงานและส่งกลับอุปกรณ์ไปยังการตั้งค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="8a4a4-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="8a4a4-104">ลงชื่อเข้าใช้การจัดการอุปกรณ์ของ Microsoft ๓๖๕แล้วไปที่**อุปกรณ์**  >  **ทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="8a4a4-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="8a4a4-105">เลือกอุปกรณ์ที่คุณต้องการลบข้อมูล</span><span class="sxs-lookup"><span data-stu-id="8a4a4-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="8a4a4-106">เลือกชนิดของการล้างข้อมูลระยะไกลที่คุณต้องการทำ</span><span class="sxs-lookup"><span data-stu-id="8a4a4-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="8a4a4-107">ถอนการลบเฉพาะข้อมูลขององค์กรเท่านั้นในขณะที่การลบข้อมูลทั้งหมดจะคืนค่าอุปกรณ์ไปยังการตั้งค่าจากโรงงาน</span><span class="sxs-lookup"><span data-stu-id="8a4a4-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="8a4a4-108">เลือก **ใช่** เพื่อยืนยัน</span><span class="sxs-lookup"><span data-stu-id="8a4a4-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="8a4a4-109">จนกว่าการลบจะเสร็จสิ้นสถานะการดำเนินการของอุปกรณ์จะแสดงเป็นออกจากระหว่างการดำเนินการ</span><span class="sxs-lookup"><span data-stu-id="8a4a4-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="8a4a4-110">หลังจากที่การดำเนินการเสร็จสมบูรณ์แล้วคุณจะไม่เห็นอุปกรณ์เคลื่อนที่ในรายการของอุปกรณ์ที่มีการจัดการอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="8a4a4-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="8a4a4-111">**หมายเหตุ:** ข้อมูลบริษัทไม่สามารถเอาออกจากอุปกรณ์ที่เข้าร่วมกับ Azure AD ได้</span><span class="sxs-lookup"><span data-stu-id="8a4a4-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="8a4a4-112">สำหรับรายละเอียดทั้งหมดของผลกระทบของการดำเนินการถอนและล้างข้อมูลรวมถึงสิ่งที่ถูกเก็บไว้และสิ่งที่ถูกลบออกให้ดูที่[เอาอุปกรณ์ออกโดยใช้การลบออกหรือด้วยตนเอง unenrolling อุปกรณ์](https://docs.microsoft.com/intune/devices-wipe)</span><span class="sxs-lookup"><span data-stu-id="8a4a4-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="8a4a4-113">เมื่อต้องการลบข้อมูลทั้งหมดออกจากอุปกรณ์ macOS ให้ดูที่[ลบข้อมูลทั้งหมดออกจากอุปกรณ์ macOS](https://docs.microsoft.com/intune/device-erase)</span><span class="sxs-lookup"><span data-stu-id="8a4a4-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>