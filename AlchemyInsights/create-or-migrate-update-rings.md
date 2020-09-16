---
title: การสร้างหรือโยกย้ายการอัปเดตวงแหวน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1126"
- "6700007"
ms.openlocfilehash: 06f905551cbd015c80b6de4f97d0beb535d70fa0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732374"
---
# <a name="create-or-migrate-update-rings"></a><span data-ttu-id="d2a93-102">การสร้างหรือโยกย้ายการอัปเดตวงแหวน</span><span class="sxs-lookup"><span data-stu-id="d2a93-102">Create or migrate update rings</span></span>

<span data-ttu-id="d2a93-103">ถ้าคุณกำหนดค่า Windows 10 การตั้งค่าการอัปเดตในพอร์ทัลของ Intune classic และคุณต้องการโยกย้ายการตั้งค่าไปยัง Intune ในพอร์ทัล Azure ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d2a93-103">If you configured Windows 10 update settings in the Intune classic portal and you want to migrate the settings to Intune in the Azure portal, follow these steps:</span></span>

1.  <span data-ttu-id="d2a93-104">ไปที่พอร์ทัล Azure และเลือก**บริการทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="d2a93-104">Go to the Azure portal and select  **All Services**.</span></span>
2.  <span data-ttu-id="d2a93-105">ในเขตข้อมูล**ตัวกรอง**ให้พิมพ์**Intune**แล้วเลือก**Microsoft Intune**</span><span class="sxs-lookup"><span data-stu-id="d2a93-105">In the  **Filter**  field, type  **Intune**, and choose  **Microsoft Intune**.</span></span>
3.  <span data-ttu-id="d2a93-106">เลือกการ**อัปเดตซอฟต์แวร์**   >   **Windows 10 ปรับปรุง**การ   >   **สร้าง**วงแหวน</span><span class="sxs-lookup"><span data-stu-id="d2a93-106">Select  **Software updates**  >  **Windows 10 Update Rings**  >  **Create**.</span></span>
4.  <span data-ttu-id="d2a93-107">ใส่ชื่อและคำอธิบายแล้วเลือก**กำหนดค่า**</span><span class="sxs-lookup"><span data-stu-id="d2a93-107">Enter a name and description, and select  **Configure**.</span></span>
5.  <span data-ttu-id="d2a93-108">กำหนดค่าการตั้งค่าการอัปเดตซอฟต์แวร์สำหรับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="d2a93-108">Configure the software update settings for your organization.</span></span>
6.  <span data-ttu-id="d2a93-109">เลือก**ตกลง**  >  **สร้างวงแหวนอัปเดต**  >  **Create**</span><span class="sxs-lookup"><span data-stu-id="d2a93-109">Select  **OK** > **Create Update Ring** > **Create**.</span></span>