---
title: หยุดข้อความจากการย้ายไปยังที่เก็บถาวรโดยอัตโนมัติ
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527753"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="94835-102">หยุดข้อความจากการย้ายไปยังที่เก็บถาวรโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="94835-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="94835-103">ถ้าคุณใช้นโยบายการเก็บข้อมูล คุณสามารถเปลี่ยนอายุการเก็บข้อมูลในนโยบายนั้นเพื่อหยุดการเก็บถาวรข้อความโดยอัตโนมัติได้</span><span class="sxs-lookup"><span data-stu-id="94835-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="94835-104">โดยมีวิธีการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="94835-104">Here's how:</span></span>

1. <span data-ttu-id="94835-105">ในศูนย์ [การจัดการ Exchange ให้เลือก](https://go.microsoft.com/fwlink/?linkid=2059104)แท็ก **การเก็บข้อมูล**  >  **การจัดการการปฏิบัติตาม** นโยบาย</span><span class="sxs-lookup"><span data-stu-id="94835-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="94835-106">ค้นหาแท็กการเก็บข้อมูล ย้ายไปยังที่เก็บถาวร ของคุณ</span><span class="sxs-lookup"><span data-stu-id="94835-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="94835-107">ในแท็กการเก็บข้อมูล ให้เปลี่ยนช่วงเวลาการเก็บข้อมูล (ช่วงเวลาการเก็บถาวร) เป็น ไม่หยุดการเก็บถาวรรายการโดยนโยบายการเก็บข้อมูลโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="94835-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="94835-108">นี่จะเปลี่ยนการตั้งค่าการเก็บถาวรของกล่องจดหมายทั้งหมดที่แท็กการเก็บข้อมูลนี้ใช้กับกล่องจดหมายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="94835-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
