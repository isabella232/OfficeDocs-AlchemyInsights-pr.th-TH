---
title: ใช้การป้องกันการติดตามใน Microsoft Edge (Chromium)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8328"
- "10979"
- "9004625"
- "9006450"
ms.openlocfilehash: beaa5dcc7f2e07ca3b2339fe43a759acf3a342b0
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989880"
---
# <a name="use-tracking-prevention-in-microsoft-edge-chromium"></a><span data-ttu-id="a5648-102">ใช้การป้องกันการติดตามใน Microsoft Edge (Chromium)</span><span class="sxs-lookup"><span data-stu-id="a5648-102">Use tracking prevention in Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="a5648-103">บางเว็บไซต์จะใช้ตัวติดตามเพื่อรวบรวมข้อมูลเบราว์เซอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5648-103">Some websites use trackers to collect your browser information.</span></span> <span data-ttu-id="a5648-104">เราได้สร้างการป้องกันภายในเพื่อจํากัดการเข้าถึงการติดตามข้อมูลที่ยึดตามเบราว์เซอร์และเสนอตัวเลือกเพิ่มเติมเพื่อปรับแต่งระดับความปลอดภัยของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5648-104">We’ve built in protections to limit access to tracking browser-based info and offer additional options for you to customize your level of security.</span></span>

- <span data-ttu-id="a5648-105">**พื้นฐาน**</span><span class="sxs-lookup"><span data-stu-id="a5648-105">**Basic**.</span></span> <span data-ttu-id="a5648-106">มีข้อจํากัดน้อยที่สุดและได้รับการออกแบบมาเพื่อให้ผู้ใช้เพลิดเพลินกับโฆษณาที่ปรับให้เป็นแบบส่วนตัว และไม่ต้องกังวลว่าจะถูกติดตามบนเว็บ</span><span class="sxs-lookup"><span data-stu-id="a5648-106">Least restrictive and designed for users who enjoy personalized advertisements and don't mind being tracked on the web.</span></span> <span data-ttu-id="a5648-107">พื้นฐานจะป้องกันผู้ใช้จากตัวติดตามที่เป็นอันตราย เช่น ตัวลายนิ้วมือและตัวเข้ารหัสลับ</span><span class="sxs-lookup"><span data-stu-id="a5648-107">Basic protects users against malicious trackers, like fingerprinters and cryptominers.</span></span>
- <span data-ttu-id="a5648-108">**สมดุล**</span><span class="sxs-lookup"><span data-stu-id="a5648-108">**Balanced**.</span></span> <span data-ttu-id="a5648-109">ระดับเริ่มต้นและได้รับการออกแบบมาให้ผู้ใช้ที่ต้องการเห็นโฆษณาที่ติดตามเนื้อหารอบๆ เว็บให้น้อย</span><span class="sxs-lookup"><span data-stu-id="a5648-109">Default level and designed for users who want to see fewer advertisements that follow them around the web.</span></span> <span data-ttu-id="a5648-110">ระดับสมดุล ไม่เพียงแต่จะบล็อกตัวติดตามจากไซต์ที่ผู้ใช้ไม่เคยมีส่วนร่วมเท่านั้น แต่ยังลดความเสี่ยงของปัญหาความเข้ากันได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="a5648-110">Balanced level not only blocks trackers from sites that users never engage with but also minimizes the risk of compatibility issues.</span></span>
- <span data-ttu-id="a5648-111">**เคร่ง** ครัด</span><span class="sxs-lookup"><span data-stu-id="a5648-111">**Strict**.</span></span> <span data-ttu-id="a5648-112">มีข้อจํากัดมากที่สุดและออกแบบมาเพื่อให้ผู้ใช้ที่ไม่ระลึกถึงความเข้ากันได้ของเว็บไซต์อย่างเข้มงวดมากที่สุดเพื่อความเป็นส่วนตัวสูงสุด</span><span class="sxs-lookup"><span data-stu-id="a5648-112">Most restrictive and designed for users who don't mind sacrificing website compatibility for maximum privacy.</span></span>

<span data-ttu-id="a5648-113">หากคุณต้องการอัปเดตการตั้งค่าความเป็นส่วนตัวในเบราว์เซอร์ Microsoft Edge ให้ไปที่ **การตั้งค่า**  >  **ความเป็นส่วนตัว การค้นหา และบริการ**</span><span class="sxs-lookup"><span data-stu-id="a5648-113">If you want to update your privacy settings, in your Edge browser, go to **Settings** > **Privacy, search, and services**.</span></span> <span data-ttu-id="a5648-114">คุณสามารถอัปเดตการตั้งค่าการป้องกันการติดตาม บล็อกตัวติดตาม ล้างข้อมูลการเรียกดู และสวจตัวเลือกความเป็นส่วนตัวและความปลอดภัยอื่นๆ เพื่อเก็บข้อมูลของคุณให้ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="a5648-114">You can update your tracking prevention settings, block trackers, clear browsing data, and explore other privacy and security options to keep your data safe.</span></span> <span data-ttu-id="a5648-115">เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดูที่ การป้องกันการติดตามใน Microsoft Edge](/microsoft-edge/web-platform/tracking-prevention)</span><span class="sxs-lookup"><span data-stu-id="a5648-115">To learn more, see [Tracking Prevention in Microsoft Edge](/microsoft-edge/web-platform/tracking-prevention).</span></span> 