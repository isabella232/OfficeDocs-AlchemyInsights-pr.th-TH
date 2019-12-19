---
title: มีข้อผิดพลาดเกิดขึ้นในการตรวจสอบข้อผิดพลาดโทเค็นการเข้าถึงระหว่างการวิเคราะห์บนเดสก์ท็อป
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741292"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="2ce27-102">เกิดข้อผิดพลาด "มีข้อผิดพลาดในการตรวจสอบโทเค็นการเข้าถึง" ระหว่างการเตรียมใช้งาน Analytics บนเดสก์ท็อป</span><span class="sxs-lookup"><span data-stu-id="2ce27-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="2ce27-103">โดยปกติแล้วข้อผิดพลาดนี้จะสังเกตเห็นเมื่อโทเค็นการรับรองความถูกต้องหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="2ce27-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="2ce27-104">โดยปกติแล้วการรีเฟรชหน้าเว็บจะรีเฟรชโทเค็น</span><span class="sxs-lookup"><span data-stu-id="2ce27-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="2ce27-105">อย่างไรก็ตามปัญหานี้สามารถยังคงมีอยู่ถ้ามีนโยบายการเข้าถึงแบบมีเงื่อนไขใดๆที่ใช้กับบัญชีที่ใช้ในการวิเคราะห์บนเดสก์ท็อปบนกระดาน</span><span class="sxs-lookup"><span data-stu-id="2ce27-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="2ce27-106">คุณสามารถตรวจสอบแฟ้มบันทึกการเข้าสู่ระบบ AD Azure ในเว็บไซต์ Azure เพื่อดูว่ามีความล้มเหลวในการลงชื่อเข้าใช้สำหรับบัญชีผู้ใช้สำหรับการเตรียมการของ Analytics บนเดสก์ท็อปหรือไม่</span><span class="sxs-lookup"><span data-stu-id="2ce27-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="2ce27-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้เยี่ยมชม[แผนการปรับใช้การเข้าถึงแบบมีเงื่อนไขของคุณ](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="2ce27-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>