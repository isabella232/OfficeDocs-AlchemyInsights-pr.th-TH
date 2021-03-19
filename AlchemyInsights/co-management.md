---
title: การจัดการร่วม
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: a10f2d9ee8617cf194c61492be69064d53242318
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "50896814"
---
# <a name="co-management"></a><span data-ttu-id="29bc6-102">การจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="29bc6-102">Co-management</span></span>

<span data-ttu-id="29bc6-103">**เงื่อนไขเบื้องต้นในการโยกย้ายจาก Config Manager แบบไฮบริดไปยัง Intuny**</span><span class="sxs-lookup"><span data-stu-id="29bc6-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="29bc6-104">อ่าน[บทความนี้](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)</span><span class="sxs-lookup"><span data-stu-id="29bc6-104">Review [this article](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid).</span></span>
- <span data-ttu-id="29bc6-105">[เพิ่มสิทธิ์การใช้งาน Intun1 ให้กับผู้ใช้](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="29bc6-105">[Add an Intune license to your users](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign).</span></span>
- <span data-ttu-id="29bc6-106">ใช้ [เบราว์เซอร์ Microsoft Edge](https://www.microsoft.com/edge) เมื่อกําหนดค่าการจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="29bc6-106">Use the [Edge browser](https://www.microsoft.com/edge) when configuring Co-management.</span></span>

<span data-ttu-id="29bc6-107">ประสบการณ์การตั้งค่าการจัดการร่วมแบบทีละขั้นตอนสามารถพบ[ได้ที่นี่](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide)</span><span class="sxs-lookup"><span data-stu-id="29bc6-107">A guided, step-by-step Co-management setup experience can be found [here](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide).</span></span>

<span data-ttu-id="29bc6-108">**How to I install the Config Manager client on Intune-managed devices**</span><span class="sxs-lookup"><span data-stu-id="29bc6-108">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="29bc6-109">ดู[อุปกรณ์ Windows ที่จัดการโดย Intun1 MDM](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="29bc6-109">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="29bc6-110">**จะเกิดอะไรขึ้นถ้าฉันต้องการเปลี่ยนอํานาจของ MDM**</span><span class="sxs-lookup"><span data-stu-id="29bc6-110">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="29bc6-111">MDM Authority สามารถเปลี่ยนแปลงได้โดยไม่ต้องเปิดกรณีการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="29bc6-111">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="29bc6-112">โปรดตรวจทานเอกสารประกอบต่อไปนี้เพื่อช่วยในการเปลี่ยนผู้ออกใบรับรอง MDM ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="29bc6-112">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="29bc6-113">เปลี่ยนผู้ให้บริการออก MDM จากตัวจัดการการกําหนดค่าเป็น Intun1 แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="29bc6-113">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
- [<span data-ttu-id="29bc6-114">เปลี่ยนผู้ให้บริการ MDM จาก Intun1 แบบสแตนด์อโลนเป็นตัวจัดการการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="29bc6-114">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
