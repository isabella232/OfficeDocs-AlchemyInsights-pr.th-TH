---
title: การจัดการร่วม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: 0f7c5d647e133b092b778c39fddc3c3ae3e7c7fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681279"
---
# <a name="co-management"></a><span data-ttu-id="8425e-102">การจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="8425e-102">Co-management</span></span>

<span data-ttu-id="8425e-103">**ข้อกำหนดเบื้องต้นสำหรับการโยกย้ายจากไฮบริดของตัวจัดการ Config เป็น Intune**</span><span class="sxs-lookup"><span data-stu-id="8425e-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="8425e-104">ตรวจทาน[บทความนี้](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-hybridmdm-to-intunesa)</span><span class="sxs-lookup"><span data-stu-id="8425e-104">Review [this article](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="8425e-105">[เพิ่มสิทธิ์การใช้งาน Intune ให้กับผู้ใช้ของคุณ](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="8425e-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="8425e-106">ใช้ [เบราว์เซอร์ Edge](https://www.microsoft.com/windows/microsoft-edge) เมื่อกำหนดค่าการจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="8425e-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="8425e-107">**ฉันจะติดตั้งไคลเอ็นต์ตัวจัดการการกำหนดค่าบนอุปกรณ์ที่มีการจัดการ Intune ได้อย่างไร**</span><span class="sxs-lookup"><span data-stu-id="8425e-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="8425e-108">ดู [อุปกรณ์ Windows](https://docs.microsoft.com/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)ที่ได้รับการจัดการด้วย MDM</span><span class="sxs-lookup"><span data-stu-id="8425e-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="8425e-109">**จะเกิดอะไรขึ้นถ้าฉันต้องการเปลี่ยนแปลงสิทธิ์ MDM**</span><span class="sxs-lookup"><span data-stu-id="8425e-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="8425e-110">สิทธิ์การใช้งาน MDM สามารถเปลี่ยนแปลงได้โดยไม่ต้องเปิดกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="8425e-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="8425e-111">โปรดตรวจทานเอกสารต่อไปนี้เพื่อช่วยในการเปลี่ยนแปลงสิทธิ์การใช้งาน MDM ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="8425e-111">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="8425e-112">การเปลี่ยนแปลงสิทธิ์ MDM จากตัวจัดการการกำหนดค่าไปยัง Intune แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="8425e-112">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="8425e-113">การเปลี่ยนแปลงสิทธิ์ MDM จาก Intune แบบสแตนด์อโลนไปยังตัวจัดการการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="8425e-113">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/change-mdm-authority)
