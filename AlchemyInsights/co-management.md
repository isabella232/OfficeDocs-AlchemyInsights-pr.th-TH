---
title: การจัดการร่วม
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: c7dc35a484894e147208ef7080c151c6d3af0c63
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817731"
---
# <a name="co-management"></a><span data-ttu-id="94098-102">การจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="94098-102">Co-management</span></span>

<span data-ttu-id="94098-103">**เบื้องต้นในการโยกย้ายจาก Config Manager แบบไฮบริดเป็น Intuny**</span><span class="sxs-lookup"><span data-stu-id="94098-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="94098-104">[อ่าน](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)บทความนี้</span><span class="sxs-lookup"><span data-stu-id="94098-104">Review [this article](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid).</span></span>
- <span data-ttu-id="94098-105">[เพิ่มสิทธิ์การใช้งาน Intun1 ให้กับผู้ใช้](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)ของคุณ</span><span class="sxs-lookup"><span data-stu-id="94098-105">[Add an Intune license to your users](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign).</span></span>
- <span data-ttu-id="94098-106">ใช้เบราว์เซอร์ [Microsoft Edge](https://www.microsoft.com/edge) เมื่อกําหนดค่าการจัดการร่วม</span><span class="sxs-lookup"><span data-stu-id="94098-106">Use the [Edge browser](https://www.microsoft.com/edge) when configuring Co-management.</span></span>

<span data-ttu-id="94098-107">ประสบการณ์การตั้งค่าการจัดการร่วมแบบทีละขั้นตอนแบบทีละขั้นตอน[สามารถพบได้ที่นี่](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide)</span><span class="sxs-lookup"><span data-stu-id="94098-107">A guided, step-by-step Co-management setup experience can be found [here](https://admin.microsoft.com/AdminPortal/Home?#/modernonboarding/comanagesetupguide).</span></span>

<span data-ttu-id="94098-108">**ฉันจะติดตั้งไคลเอ็นต์ Config Manager บนอุปกรณ์ที่มีการจัดการ Intun <2>**</span><span class="sxs-lookup"><span data-stu-id="94098-108">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="94098-109">ดู[อุปกรณ์ Windows ที่มีการจัดการโดย Intun1 MDM](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)</span><span class="sxs-lookup"><span data-stu-id="94098-109">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/mem/configmgr/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="94098-110">**จะเกิดอะไรขึ้นถ้าฉันต้องการเปลี่ยนอํานาจ MDM**</span><span class="sxs-lookup"><span data-stu-id="94098-110">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="94098-111">MDM Authority สามารถเปลี่ยนแปลงได้โดยไม่ต้องเปิดกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="94098-111">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="94098-112">โปรดตรวจทานเอกสารประกอบต่อไปนี้เพื่อช่วยในการเปลี่ยนอํานาจของ MDM ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="94098-112">Please review the following documentation to assist in changing your MDM authority:</span></span>

- [<span data-ttu-id="94098-113">เปลี่ยนผู้ให้บริการออก MDM จากตัวจัดการการกําหนดค่าเป็น Intuny แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="94098-113">Change MDM Authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
- [<span data-ttu-id="94098-114">เปลี่ยนผู้ให้บริการ MDM จาก Intuny แบบสแตนด์อโลนเป็นตัวจัดการการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="94098-114">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/mem/configmgr/mdm/understand/what-happened-to-hybrid)
