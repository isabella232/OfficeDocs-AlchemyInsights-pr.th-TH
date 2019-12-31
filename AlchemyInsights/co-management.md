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
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910476"
---
# <a name="co-management"></a><span data-ttu-id="ed289-102">การจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="ed289-102">Co-management</span></span>

<span data-ttu-id="ed289-103">**ข้อกำหนดเบื้องต้นสำหรับการย้ายจากตัวจัดการการกำหนดค่าไฮบริดสลีไป Intune**</span><span class="sxs-lookup"><span data-stu-id="ed289-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="ed289-104">ทบทวน[บทความนี้](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)</span><span class="sxs-lookup"><span data-stu-id="ed289-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="ed289-105">[เพิ่มใบอนุญาต Intune ให้กับผู้ใช้ของคุณ](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="ed289-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="ed289-106">ใช้[เบราว์เซอร์ขอบ](https://www.microsoft.com/windows/microsoft-edge)เมื่อกำหนดค่าการจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="ed289-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="ed289-107">**วิธีการติดตั้งไคลเอนต์จัดการการกำหนดค่าบนอุปกรณ์ที่จัดการ Intune**</span><span class="sxs-lookup"><span data-stu-id="ed289-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="ed289-108">ดู[อุปกรณ์ Windows ที่มีจัดการ MDM แบบ Intune](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="ed289-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="ed289-109">**จะเกิดอะไรขึ้นถ้าฉันต้องการเปลี่ยนแปลงหน่วยงาน MDM**</span><span class="sxs-lookup"><span data-stu-id="ed289-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="ed289-110">สามารถเปลี่ยนแปลงได้โดยไม่ต้องเปิดกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ed289-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="ed289-111">โปรดตรวจทานเอกสารต่อไปนี้เพื่อช่วยในการเปลี่ยนแปลงหน่วยงาน MDM ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="ed289-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="ed289-112">เปลี่ยน MDM หน่วยงานจากตัวจัดการการกำหนดค่าเป็น Intune แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="ed289-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="ed289-113">เปลี่ยนแปลงการทำงานของ MDM จาก Intune แบบสแตนด์อโลนไปยังตัวจัดการการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="ed289-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)