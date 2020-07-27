---
title: สร้างหรือย้ายเสียงเรียกเข้าของการอัพเดต
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1126"
- "6700007"
ms.openlocfilehash: 87102d7809d298531b5655559364c9df22e8eb91
ms.sourcegitcommit: 3fa780811984400c525d66edf46a3196f6290df0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/23/2020
ms.locfileid: "45424103"
---
# <a name="create-or-migrate-update-rings"></a><span data-ttu-id="bc857-102">สร้างหรือย้ายเสียงเรียกเข้าของการอัพเดต</span><span class="sxs-lookup"><span data-stu-id="bc857-102">Create or migrate update rings</span></span>

<span data-ttu-id="bc857-103">ถ้าคุณกําหนดค่าการตั้งค่าการปรับปรุง Windows 10 ในพอร์ทัลแบบคลาสสิก Intunเน และคุณต้องการโยกย้ายการตั้งค่าไปยัง Intuned ในพอร์ทัล Azure ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="bc857-103">If you configured Windows 10 update settings in the Intune classic portal and you want to migrate the settings to Intune in the Azure portal, follow these steps:</span></span>

1.  <span data-ttu-id="bc857-104">ไปที่พอร์ทัล Azure และเลือก**บริการทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="bc857-104">Go to the Azure portal and select  **All Services**.</span></span>
2.  <span data-ttu-id="bc857-105">ในฟิลด์**ตัวกรอง**ให้พิมพ์**Intunหรือ Intun น**แล้วเลือก**Microsoft Intun**</span><span class="sxs-lookup"><span data-stu-id="bc857-105">In the  **Filter**  field, type  **Intune**, and choose  **Microsoft Intune**.</span></span>
3.  <span data-ttu-id="bc857-106">เลือก**การปรับปรุงซอฟต์แวร์**   >   **ของ Windows 10 ปรับปรุงวงแหวน**   >   **สร้าง**</span><span class="sxs-lookup"><span data-stu-id="bc857-106">Select  **Software updates**  >  **Windows 10 Update Rings**  >  **Create**.</span></span>
4.  <span data-ttu-id="bc857-107">ป้อนชื่อและคําอธิบาย**และเลือก**</span><span class="sxs-lookup"><span data-stu-id="bc857-107">Enter a name and description, and select  **Configure**.</span></span>
5.  <span data-ttu-id="bc857-108">กําหนดค่าการตั้งค่าการปรับปรุงซอฟต์แวร์สําหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="bc857-108">Configure the software update settings for your organization.</span></span>
6.  <span data-ttu-id="bc857-109">เลือก**OK**  >  **สร้างแหวนอัพเดต**  >  **Create**</span><span class="sxs-lookup"><span data-stu-id="bc857-109">Select  **OK** > **Create Update Ring** > **Create**.</span></span>