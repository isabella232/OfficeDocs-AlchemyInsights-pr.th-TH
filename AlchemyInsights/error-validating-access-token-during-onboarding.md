---
title: มีข้อผิดพลาดการตรวจสอบความถูกต้องของข้อผิดพลาดโทเค็นการเข้าถึงระหว่างการวิเคราะห์เดสก์ท็อปบนบอร์ด
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813707"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="17a6f-102">ข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ระหว่างการออนบอร์ดการวิเคราะห์เดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="17a6f-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="17a6f-103">โดยปกติแล้วจะพบข้อผิดพลาดนี้เมื่อโทเค็นการรับรองความถูกต้องหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="17a6f-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="17a6f-104">โดยปกติแล้ว รีเฟรชหน้าจะรีเฟรชโทเค็น</span><span class="sxs-lookup"><span data-stu-id="17a6f-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="17a6f-105">อย่างไรก็ตาม ปัญหานี้สามารถคงอยู่ได้ถ้ามีนโยบายการเข้าถึงตามเงื่อนไขที่ปรับใช้กับบัญชีที่ใช้กับการวิเคราะห์เดสก์ท็อปบนบอร์ด</span><span class="sxs-lookup"><span data-stu-id="17a6f-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="17a6f-106">คุณสามารถตรวจทานแฟ้มบันทึกการลงชื่อเข้าใช้ Azure AD ในพอร์ทัล Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้บัญชีที่ใช้กับการออนบอร์ดบนเดสก์ท็อปหรือไม่</span><span class="sxs-lookup"><span data-stu-id="17a6f-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="17a6f-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="17a6f-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>