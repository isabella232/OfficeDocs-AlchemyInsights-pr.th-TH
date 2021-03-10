---
title: แก้ไขปัญหาเบราว์เซอร์การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9377"
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695344"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="99558-102">แก้ไขปัญหาเบราว์เซอร์การเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น</span><span class="sxs-lookup"><span data-stu-id="99558-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="99558-103">ผู้ใช้ส่วนใหญ่สามารถแก้ไขปัญหาเบราว์เซอร์ SSO อย่างราบรื่นได้โดยใช้ขั้นตอนด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="99558-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="99558-104">ตรวจสอบให้แน่ใจว่าเบราว์เซอร์ของคุณทันสมัย</span><span class="sxs-lookup"><span data-stu-id="99558-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="99558-105">ลบคุกกี้จากเบราว์เซอร์เพื่อเอาเซสชัน SSO ที่ไม่ถูกต้องออก แล้วลองเข้าสู่ระบบอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="99558-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="99558-106">ลองเข้าสู่ระบบโดยใช้เบราว์เซอร์อื่น</span><span class="sxs-lookup"><span data-stu-id="99558-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="99558-107">**ปัญหาที่ทราบเกี่ยวกับเบราว์เซอร์**</span><span class="sxs-lookup"><span data-stu-id="99558-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="99558-108">SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบน Firefox</span><span class="sxs-lookup"><span data-stu-id="99558-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="99558-109">SSO อย่างราบรื่นไม่ใช้งานใน Internet Explorer เมื่อเปิดโหมดที่ได้รับการป้องกันขั้นสูง</span><span class="sxs-lookup"><span data-stu-id="99558-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="99558-110">SSO อย่างราบรื่นไม่ใช้งานในโหมดการเรียกดูส่วนบุคคลบน Microsoft Edge (แบบดั้งเดิม)</span><span class="sxs-lookup"><span data-stu-id="99558-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="99558-111">SSO อย่างราบรื่นไม่ใช้งานบนเบราว์เซอร์อุปกรณ์เคลื่อนที่บน iOS และ Android</span><span class="sxs-lookup"><span data-stu-id="99558-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="99558-112">SSO อย่างราบรื่นสนับสนุน Microsoft Edge เวอร์ชันถัดไปโดยยึดตาม Chromium และใช้งานในโหมด InPrivate และโหมด Guest ตามการออกแบบ</span><span class="sxs-lookup"><span data-stu-id="99558-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="99558-113">**การปรึกษา**</span><span class="sxs-lookup"><span data-stu-id="99558-113">**Advisory**</span></span>

<span data-ttu-id="99558-114">เมื่อต้องการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น ให้ดูการถามตอบของ [Microsoft&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span><span class="sxs-lookup"><span data-stu-id="99558-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
