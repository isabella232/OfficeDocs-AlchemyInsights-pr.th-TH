---
title: ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678818"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="c3546-102">ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="c3546-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="c3546-103">Microsoft Edge ใช้บัญชีเริ่มต้นของระบบปฏิบัติการเพื่อลงชื่อเข้าใช้โดยอัตโนมัติตามวิธีที่อุปกรณ์ของผู้ใช้ได้รับการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="c3546-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="c3546-104">สถานการณ์สมมติของการกำหนดค่าอุปกรณ์แต่ละชนิดและกระบวนการลงชื่อเข้าใช้ของผู้ใช้ที่ขึ้นต่อกันจะอธิบายไว้ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="c3546-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="c3546-105">**อุปกรณ์คือไฮบริด/AAD-J**: ตัวเลือกนี้จะพร้อมใช้งานบน windows 10, windows ระดับล่างและเวอร์ชันของเซิร์ฟเวอร์ที่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="c3546-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c3546-106">ผู้ใช้จะได้รับการลงชื่อเข้าใช้โดยอัตโนมัติด้วยบัญชีผู้ใช้ Azure Active directory (AD)</span><span class="sxs-lookup"><span data-stu-id="c3546-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="c3546-107">**อุปกรณ์มีการเข้าร่วมโดเมน**: ตัวเลือกนี้จะพร้อมใช้งานบน windows 10, windows ระดับล่างและเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="c3546-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c3546-108">ตามค่าเริ่มต้นผู้ใช้ที่มีบัญชีโดเมนไม่ได้ลงชื่อเข้าใช้โดยอัตโนมัติ เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้โดยอัตโนมัติให้ใช้นโยบาย **ConfigureOnPremisesAccountAutoSignIn**</span><span class="sxs-lookup"><span data-stu-id="c3546-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="c3546-109">เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้โดยอัตโนมัติสำหรับผู้ใช้ที่มีบัญชีผู้ใช้ AD Azure ให้ลองใช้การเข้าร่วมอุปกรณ์ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="c3546-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="c3546-110">**บัญชีเริ่มต้นของระบบปฏิบัติการคือบัญชี Microsoft**: ตัวเลือกนี้จะพร้อมใช้งานบน WINDOWS 10 ขี่ (เวอร์ชัน๑๗๐๙, รุ่น 10.0.16299) และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="c3546-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="c3546-111">สถานการณ์สมมติไม่น่าจะเกิดขึ้นบนอุปกรณ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="c3546-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="c3546-112">อย่างไรก็ตามถ้าบัญชีเริ่มต้นของระบบปฏิบัติการเป็นบัญชี Microsoft microsoft Edge จะลงชื่อเข้าใช้โดยอัตโนมัติในผู้ใช้ด้วยบัญชี Microsoft</span><span class="sxs-lookup"><span data-stu-id="c3546-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
