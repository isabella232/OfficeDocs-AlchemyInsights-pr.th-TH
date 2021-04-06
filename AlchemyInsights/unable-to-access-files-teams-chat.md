---
title: ไม่สามารถเข้าถึงไฟล์ที่แชร์ในการแชทของ Teams ได้
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2021
ms.locfileid: "51596008"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="6cc00-102">ไม่สามารถเข้าถึงไฟล์ที่แชร์ในการแชทของ Teams ได้</span><span class="sxs-lookup"><span data-stu-id="6cc00-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="6cc00-103">ใน Microsoft Teams ไฟล์ที่แชร์โดยผู้ใช้ในหน้าต่างการแชทจะถูกเก็บไว้โดยอัตโนมัติบนไซต์ OneDrive ของผู้ใช้ที่แชร์</span><span class="sxs-lookup"><span data-stu-id="6cc00-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="6cc00-104">เมื่อผู้ใช้อื่นพยายามเปิดไฟล์ใน Teams และได้รับข้อความแสดงข้อผิดพลาด "คุณไม่มีสิทธิ์เข้าถึงไฟล์นี้" ปัญหานี้จะเกิดขึ้นเนื่องจากฟีเจอร์โหมดการจํากัดการเข้าถึงของผู้ใช้ถูกเปิดใช้งานบนไซต์ OneDrive ของคุณ</span><span class="sxs-lookup"><span data-stu-id="6cc00-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="6cc00-105">หากต้องการคําแนะนําในการปิดใช้งานฟีเจอร์บนไซต์ OneDrive[ให้ดูข้อผิดพลาดเมื่อเปิดไฟล์ใน Teams](https://go.microsoft.com/fwlink/?linkid=2155733)</span><span class="sxs-lookup"><span data-stu-id="6cc00-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="6cc00-106">ตรวจสอบว่าผู้ใช้อื่นมีสิทธิ์เข้าถึงไซต์ OneDrive หรือไม่ และให้สิทธิ์การเข้าถึงโดยการปฏิบัติตามคําแนะนําใน[แชร์ไฟล์และโฟลเดอร์ OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017)</span><span class="sxs-lookup"><span data-stu-id="6cc00-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>