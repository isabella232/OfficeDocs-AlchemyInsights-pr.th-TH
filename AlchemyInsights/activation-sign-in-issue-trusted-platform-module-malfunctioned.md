---
title: ปัญหาการเปิดใช้งาน/การลงชื่อเข้าใช้ - โมดูลแพลตฟอร์มที่เชื่อถือได้ผิดปกติ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822906"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="31b4b-102">การแก้ไขข้อความ "โมดูลแพลตฟอร์มที่เชื่อถือได้ของคอมพิวเตอร์ของคุณมีฟังก์ชันการฟังก์ชันไม่ถูกต้อง" ของแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="31b4b-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="31b4b-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="31b4b-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="31b4b-104">เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="31b4b-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="31b4b-105">การใช้บัญชี **บัญชี**  >  **การตั้งค่า**  >  **Windows &อีเมล** ลบบัญชีที่งานที่มีอยู่ออก</span><span class="sxs-lookup"><span data-stu-id="31b4b-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove existing work accounts.</span></span> 
3. <span data-ttu-id="31b4b-106">การใช้ บัญชี **การตั้งค่า** Windows  >    >  **เข้าถึงบัญชีที่โรงเรียน** หรือที่โรงเรียน ยกเลิกการเชื่อมต่อบัญชีที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="31b4b-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect existing accounts.</span></span> 
4. <span data-ttu-id="31b4b-107">รีเซ็ตสถานะการเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="31b4b-107">Reset Office activation state.</span></span> <span data-ttu-id="31b4b-108">[เรียนรู้วิธีการ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)</span><span class="sxs-lookup"><span data-stu-id="31b4b-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="31b4b-109">ลองกระบวนการ [กู้คืนผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของ Trusted Platform Module (TPM)</span><span class="sxs-lookup"><span data-stu-id="31b4b-109">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>