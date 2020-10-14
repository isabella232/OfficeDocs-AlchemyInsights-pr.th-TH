---
title: วิธีการสร้างหรือโยกย้ายการอัปเดตวงแหวน
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "6718"
- "9003773"
ms.openlocfilehash: 0d43e2d5a87e4b941fcc91671b41ea0aabc5bffe
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461987"
---
# <a name="how-to-create-or-migrate-update-rings"></a><span data-ttu-id="72785-102">วิธีการสร้างหรือโยกย้ายการอัปเดตวงแหวน</span><span class="sxs-lookup"><span data-stu-id="72785-102">How to create or migrate update rings</span></span>

<span data-ttu-id="72785-103">โปรดทำตามขั้นตอนด้านล่างถ้าคุณกำหนดค่าการตั้งค่าการอัปเดต Windows 10 ในพอร์ทัลคลาสสิกของ Intune และต้องการโยกย้ายไฟล์เหล่านั้นไปยัง Intune ในพอร์ทัล Azure:</span><span class="sxs-lookup"><span data-stu-id="72785-103">Please follow the steps below if you configured Windows 10 update settings in the Intune classic portal and wanted to migrate them to Intune in the Azure portal:</span></span>

1. <span data-ttu-id="72785-104">ไปที่พอร์ทัล Azure แล้วคลิก**บริการทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="72785-104">Go to the Azure portal and click **All Services**.</span></span>
2. <span data-ttu-id="72785-105">ในเขตข้อมูล**ตัวกรอง**ให้พิมพ์**Intune**</span><span class="sxs-lookup"><span data-stu-id="72785-105">In the **Filter** field, type **Intune**.</span></span> <span data-ttu-id="72785-106">ในผลลัพธ์ให้คลิก**Microsoft Intune**</span><span class="sxs-lookup"><span data-stu-id="72785-106">In the results, click **Microsoft Intune**.</span></span>
3. <span data-ttu-id="72785-107">คลิกการ**อัปเดตซอฟต์แวร์**  >  **Windows 10 ปรับปรุงการสร้างวงแหวน**  >  **Create**</span><span class="sxs-lookup"><span data-stu-id="72785-107">Click **Software updates** > **Windows 10 Update Rings** > **Create**.</span></span>
4. <span data-ttu-id="72785-108">ใส่ชื่อคำอธิบายและคลิก**กำหนดค่า**</span><span class="sxs-lookup"><span data-stu-id="72785-108">Enter a name, description, and click **Configure**.</span></span>
5. <span data-ttu-id="72785-109">กำหนดค่าการตั้งค่าการอัปเดตซอฟต์แวร์องค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="72785-109">Configure your organizations software update settings.</span></span>
6. <span data-ttu-id="72785-110">เลือก**ตกลง**</span><span class="sxs-lookup"><span data-stu-id="72785-110">Select **OK**.</span></span>
7. <span data-ttu-id="72785-111">ใน**สร้างวงแหวนอัปเดต**ให้เลือก**สร้าง**</span><span class="sxs-lookup"><span data-stu-id="72785-111">In **Create Update Ring**, select **Create**.</span></span>
