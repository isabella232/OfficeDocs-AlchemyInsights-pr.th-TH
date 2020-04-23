---
title: 182 โปรดเรียกใช้ SaRA เพื่อวินิจฉัย และแก้ไขปัญหาการตรวจสอบความถูกต้องของ Outlook
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: e14042fa80be802e646db4e30cd3d5b69b81a1d3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43765561"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="d30c7-102">ใช้ SaRA เพื่อวินิจฉัย และแก้ไขปัญหาการรับรองความถูกต้องของ Outlook</span><span class="sxs-lookup"><span data-stu-id="d30c7-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="d30c7-103">**หมายเหตุ**: โปรดตรวจสอบเพื่อดูว่า[ค่าเริ่มต้นความปลอดภัย](https://aka.ms/securitydefaults)เปิดใช้งานสําหรับองค์กรของคุณหรือไม่</span><span class="sxs-lookup"><span data-stu-id="d30c7-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="d30c7-104">ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และ Outlook ของคุณกําลังถามคุณซ้ํา ๆ สําหรับรหัสผ่าน คุณอาจเปิดใช้**ค่าเริ่มต้นการรักษาความปลอดภัย**ในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="d30c7-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="d30c7-105">เราขอแนะนําให้คุณใช้[Outlook จะถามการวินิจฉัยรหัสผ่านของฉัน](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy)บนเครื่องที่ได้รับผลกระทบเพื่อแก้ไขปัญหาที่ Outlook พร้อมท์สําหรับรหัสผ่านอย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="d30c7-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="d30c7-106">การวินิจฉัย[SaRA](https://diagnostics.office.com/#/)นี้จะไม่ตรวจสอบโดยอัตโนมัติ และส่งกลับการแก้ไขปัญหาที่เป็นไปได้สําหรับคุณที่จะใช้เพื่อแก้ไขปัญหาที่ตรวจพบใด ๆ</span><span class="sxs-lookup"><span data-stu-id="d30c7-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
