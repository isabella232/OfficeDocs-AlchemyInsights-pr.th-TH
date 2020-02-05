---
title: การจัดการร่วม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: bd19ae3bfdf5005fe4e495e78749a393128a2184
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770910"
---
# <a name="co-management"></a><span data-ttu-id="56510-102">การจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="56510-102">Co-management</span></span>

<span data-ttu-id="56510-103">**ข้อกำหนดเบื้องต้นสำหรับการโยกย้ายจากไฮบริดสลีตัวจัดการ Config เพื่อ Intune**</span><span class="sxs-lookup"><span data-stu-id="56510-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="56510-104">ตรวจทาน[บทความนี้](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-hybridmdm-to-intunesa)</span><span class="sxs-lookup"><span data-stu-id="56510-104">Review [this article](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="56510-105">[เพิ่มสิทธิ์การใช้งาน Intune ให้กับผู้ใช้ของคุณ](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="56510-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="56510-106">ใช้[เบราว์เซอร์ขอบ](https://www.microsoft.com/windows/microsoft-edge)เมื่อกำหนดค่าการจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="56510-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="56510-107">**วิธีการที่ฉันติดตั้งไคลเอ็นต์ของตัวจัดการการกำหนดค่าบนอุปกรณ์ที่มีการจัดการ Intune**</span><span class="sxs-lookup"><span data-stu-id="56510-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="56510-108">ดู[อุปกรณ์ Windows ที่จัดการโดย MDM](https://docs.microsoft.com/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="56510-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="56510-109">**จะทำอย่างไรถ้าฉันต้องการเปลี่ยนแปลงหน่วยงาน MDM**</span><span class="sxs-lookup"><span data-stu-id="56510-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="56510-110">สามารถเปลี่ยนแปลงหน่วยงาน MDM ได้โดยไม่ต้องเปิดเคสสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="56510-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="56510-111">โปรดตรวจทานเอกสารต่อไปนี้เพื่อช่วยในการเปลี่ยนแปลงหน่วยงาน MDM ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="56510-111">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="56510-112">การเปลี่ยนแปลงสิทธิ์ MDM จากตัวจัดการการตั้งค่าคอนฟิกไปยัง Intune แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="56510-112">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="56510-113">การเปลี่ยนแปลงสิทธิ์ของ MDM จาก Intune แบบสแตนด์อโลนกับตัวจัดการการตั้งค่าคอนฟิก</span><span class="sxs-lookup"><span data-stu-id="56510-113">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/change-mdm-authority)
