---
title: แก้ไขปัญหาเกี่ยวกับ Bluetooth ใน Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812951"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="04857-102">แก้ไขปัญหาเกี่ยวกับ Bluetooth ใน Windows 10</span><span class="sxs-lookup"><span data-stu-id="04857-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="04857-103">หากไอคอน Bluetooth หายไป หรือไม่สามารถเปิดหรือปิด Bluetooth ได้ คุณอาจต้องการเรียกใช้ตัวแก้ไขปัญหา Bluetooth</span><span class="sxs-lookup"><span data-stu-id="04857-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="04857-104">[เปิดการตั้งค่า แก้ไขปัญหา](ms-settings:troubleshoot)คลิก **Bluetooth** **ภายใต้ ค้นหาและแก้ไขปัญหา** อื่นๆ **คลิก เรียกใช้ตัว** แก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="04857-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="04857-105">ถ้าคุณไม่เห็นไอคอน Bluetooth แต่ Bluetooth ปรากฏในตัวจัดการอุปกรณ์:</span><span class="sxs-lookup"><span data-stu-id="04857-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="04857-106">ใน ตัวจัดการอุปกรณ์ ให้คลิก **Bluetooth**</span><span class="sxs-lookup"><span data-stu-id="04857-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="04857-107">กดค้างไว้ (หรือคลิกขวา) ที่ชื่ออะแดปเตอร์ Bluetooth **แล้วคลิก ถอนการติดตั้ง** อุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="04857-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="04857-108">ปิดอุปกรณ์ Windows ของคุณ รอสักครู่ แล้วเปิดเครื่องอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="04857-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="04857-109">Windows จะพยายามติดตั้งโปรแกรมควบคุมอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="04857-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="04857-110">ถ้าคุณเพิ่งติดตั้งการอัปเดต Windows 10 หรืออัปเกรดเป็น Windows 10 คุณอาจต้องการตรวจหาการอัปเดตโปรแกรมควบคุม:</span><span class="sxs-lookup"><span data-stu-id="04857-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="04857-111">ใน ตัวจัดการอุปกรณ์ ให้คลิก **Bluetooth** แล้วคลิกชื่ออะแดปเตอร์ Bluetooth (ซึ่งอาจมีข้อความ "วิทยุ")</span><span class="sxs-lookup"><span data-stu-id="04857-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="04857-112">กด (หรือคลิกขวา) อะแดปเตอร์ Bluetooth ค้างไว้ แล้วคลิก อัปเดตการค้นหา  >  **โปรแกรมควบคุมโดยอัตโนมัติเพื่อค้นหาซอฟต์แวร์โปรแกรมควบคุมที่** อัปเดตแล้ว</span><span class="sxs-lookup"><span data-stu-id="04857-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="04857-113">Follow the steps, then click **Close**.</span><span class="sxs-lookup"><span data-stu-id="04857-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="04857-114">หาก Windows ไม่พบโปรแกรมควบคุม Bluetooth ใหม่ ให้เยี่ยมชมเว็บไซต์ของผู้ผลิตพีซี และดาวน์โหลดโปรแกรมควบคุม Bluetooth ล่าสุดจากที่นั่น</span><span class="sxs-lookup"><span data-stu-id="04857-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="04857-115">หลังจากที่คุณดาวน์โหลดแล้ว ให้คลิกอัปเดตโปรแกรมควบคุม เรียกดูซอฟต์แวร์โปรแกรมควบคุมของคอมพิวเตอร์ของฉัน เรียกดูสถานที่ที่จัดเก็บไฟล์โปรแกรมควบคุมไว้ > ตกลง ถัดไป แล้วปฏิบัติตามขั้นตอน  >    >    >  เพื่อติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="04857-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="04857-116">หลังจากติดตั้งโปรแกรมควบคุมที่อัปเดตแล้ว ให้รีสตาร์ตเครื่อง แล้วตรวจสอบว่าสามารถแก้ไขปัญหาการเชื่อมต่อหรือไม่</span><span class="sxs-lookup"><span data-stu-id="04857-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="04857-117">หากต้องการรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการแก้ไขปัญหาเกี่ยวกับ Bluetooth โปรดดูบทความฉบับเต็ม[ที่ชื่อ แก้ไขปัญหา Bluetooth ใน Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="04857-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
