---
title: การเปิดใช้งาน/ปัญหาในการลงชื่อเข้าใช้-โมดูลของ platform ที่เชื่อถือได้ปกติ
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
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697540"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="9d6df-102">การแก้ไขแอป Microsoft ๓๖๕ "โมดูลของ Platform ที่เชื่อถือได้ของคอมพิวเตอร์ของคุณไม่ทำงานอย่างถูกต้อง"</span><span class="sxs-lookup"><span data-stu-id="9d6df-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="9d6df-103">เมื่อต้องการแก้ไขข้อผิดพลาดนี้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9d6df-103">To fix this error, try the following:</span></span>

1. <span data-ttu-id="9d6df-104">เปิดแอป Office และ [ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) จากบัญชีผู้ใช้ใดๆที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="9d6df-104">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>   
2. <span data-ttu-id="9d6df-105">การใช้**การตั้งค่า**Windows บัญชีผู้ใช้  >  **Accounts**  >  **อีเมลของ**บัญชีผู้ใช้ & เอาบัญชีที่ทำงานที่มีอยู่ออก</span><span class="sxs-lookup"><span data-stu-id="9d6df-105">Using Windows **Settings** > **Accounts** > **Email & accounts**, remove existing work accounts.</span></span> 
3. <span data-ttu-id="9d6df-106">การใช้**การตั้งค่า**Windows  >  **Accounts**  >  Access บัญชีที่**ทำงานหรือโรงเรียน**ให้ยกเลิกการเชื่อมต่อบัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="9d6df-106">Using Windows **Settings** > **Accounts** > **Access work or school**, disconnect existing accounts.</span></span> 
4. <span data-ttu-id="9d6df-107">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="9d6df-107">Reset Office activation state.</span></span> <span data-ttu-id="9d6df-108">[เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)การ</span><span class="sxs-lookup"><span data-stu-id="9d6df-108">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).</span></span>
5. <span data-ttu-id="9d6df-109">ลอง [ใช้กระบวนการกู้คืนของผู้ใช้](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) เพื่อแก้ไขความล้มเหลวของโมดูลของ PLATFORM (TPM) ที่เชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="9d6df-109">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>