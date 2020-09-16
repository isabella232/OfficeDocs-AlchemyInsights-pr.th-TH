---
title: 'ข้อผิดพลาด: เราไม่สามารถอัปโหลดหรือดาวน์โหลดการเปลี่ยนแปลงของคุณได้เนื่องจากข้อมูลประจำตัวที่แคชไว้ของคุณหมดอายุ'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734498"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="68474-102">ข้อผิดพลาด: เราไม่สามารถอัปโหลดหรือดาวน์โหลดการเปลี่ยนแปลงของคุณได้เนื่องจากข้อมูลประจำตัวที่แคชไว้ของคุณหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="68474-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="68474-103">เมื่อบันทึกไฟล์ไปยังแอป OneDrive ถ้าคุณได้รับข้อผิดพลาดที่มีวลี **"ข้อมูลประจำตัวที่แคชไว้ของคุณหมดอายุแล้ว"** ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="68474-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="68474-104">ปิดแอปพลิเคชัน Office ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="68474-104">Close all Office applications.</span></span>
1. <span data-ttu-id="68474-105">เปิดตัวจัดการข้อมูลประจำตัวแล้วพิมพ์**ตัวจัดการข้อมูลประจำ**ตัวในกล่องค้นหาบนแถบงานจากนั้นเลือก**แผงควบคุมตัวจัดการข้อมูลประจำตัว**</span><span class="sxs-lookup"><span data-stu-id="68474-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="68474-106">เลือก**ข้อมูลประจำตัวของ Windows**</span><span class="sxs-lookup"><span data-stu-id="68474-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="68474-107">ค้นหารายการใดๆที่เริ่มต้นด้วย word **OneDrive**</span><span class="sxs-lookup"><span data-stu-id="68474-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="68474-108">เลือกรายการแล้วกด**เอาออก**</span><span class="sxs-lookup"><span data-stu-id="68474-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="68474-109">ปิดตัวจัดการข้อมูลประจำตัวจากนั้นคลิกขวาบนระบบคลาวด์สีน้ำเงินใน systray ของคุณแล้วเลือก**ปิด OneDrive**</span><span class="sxs-lookup"><span data-stu-id="68474-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="68474-110">พิมพ์ **OneDrive** ลงในกล่องค้นหาบนแถบงานแล้วเลือก **แอป onedrive** เพื่อเปิดใช้งาน onedrive</span><span class="sxs-lookup"><span data-stu-id="68474-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="68474-111">ลงชื่อเข้าใช้ OneDrive แล้วลองบันทึกไฟล์ไปยัง OneDrive</span><span class="sxs-lookup"><span data-stu-id="68474-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
