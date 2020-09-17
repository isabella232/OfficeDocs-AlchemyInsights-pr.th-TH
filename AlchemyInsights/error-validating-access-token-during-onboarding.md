---
title: มีข้อผิดพลาดในการตรวจสอบความถูกต้องของโทเค็นการเข้าถึงในระหว่างการใช้งาน Analytics บนเดสก์ท็อป
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783570"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="909fa-102">ข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ในระหว่างการปฐมนิเทศ Analytics บนเดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="909fa-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="909fa-103">ข้อผิดพลาดนี้มักจะสังเกตเมื่อโทเค็นการรับรองความถูกต้องหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="909fa-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="909fa-104">โดยปกติแล้วการรีเฟรชหน้าจะรีเฟรชโทเค็น</span><span class="sxs-lookup"><span data-stu-id="909fa-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="909fa-105">อย่างไรก็ตามปัญหานี้อาจยังคงมีอยู่ถ้ามีนโยบายการเข้าถึงตามเงื่อนไขที่นำไปใช้กับบัญชีผู้ใช้ในการวิเคราะห์บนเดสก์ท็อปบนกระดาน</span><span class="sxs-lookup"><span data-stu-id="909fa-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="909fa-106">คุณสามารถตรวจสอบการลงชื่อเข้าใช้ Azure AD ในบันทึกในพอร์ทัล Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้สำหรับบัญชีผู้ใช้สำหรับปฐมนิเทศ Analytics บนเดสก์ท็อปหรือไม่</span><span class="sxs-lookup"><span data-stu-id="909fa-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="909fa-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้เยี่ยมชม[วางแผนการปรับใช้การเข้าถึงตามเงื่อนไขของคุณ](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="909fa-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>