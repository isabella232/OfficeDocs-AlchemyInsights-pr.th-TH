---
title: ๑๘๒โปรดเรียกใช้ SaRA เพื่อวินิจฉัยและแก้ไขปัญหาเกี่ยวกับการรับรองความถูกต้องของ Outlook
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802040"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="870d4-102">ใช้ SaRA เพื่อวินิจฉัยและแก้ไขปัญหาการรับรองความถูกต้องของ Outlook</span><span class="sxs-lookup"><span data-stu-id="870d4-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="870d4-103">**หมายเหตุ**: โปรดตรวจสอบเพื่อดูว่ามีการเปิดใช้งาน [ค่าเริ่มต้นด้านความปลอดภัย](https://aka.ms/securitydefaults) สำหรับองค์กรของคุณหรือไม่</span><span class="sxs-lookup"><span data-stu-id="870d4-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="870d4-104">ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่21ตุลาคม๒๐๑๙และ Outlook ของคุณจะขอรหัสผ่านของคุณซ้ำๆคุณอาจมี **ค่าเริ่มต้นของความปลอดภัย** ที่เปิดใช้งานในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="870d4-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="870d4-105">เราขอแนะนำให้คุณใช้ Outlook เพื่อขอการวินิจฉัย [รหัสผ่านของฉัน](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) บนเครื่องจักรที่ได้รับผลกระทบเพื่อแก้ไขปัญหาที่ Outlook แสดงพร้อมท์สำหรับรหัสผ่านอย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="870d4-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="870d4-106">การ [วินิจฉัยนี้](https://diagnostics.office.com/#/) เป็นการตรวจสอบโดยอัตโนมัติและส่งกลับโซลูชันที่เป็นไปได้เพื่อให้คุณสามารถใช้เพื่อแก้ไขปัญหาการตรวจพบใดๆ</span><span class="sxs-lookup"><span data-stu-id="870d4-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
