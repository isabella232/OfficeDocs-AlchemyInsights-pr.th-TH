---
title: ไม่สามารถเข้าสู่ระบบ Teams เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932286"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="dbd4f-102">ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso ดอทคอม:443</span><span class="sxs-lookup"><span data-stu-id="dbd4f-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="dbd4f-103">ถ้า SSO แบบไม่มีรอยต่อถูกเปิดใช้งานเป็นการรับรองความถูกต้องของ O365, URL "autologon.microsoftazuread-sso.com" อาจจําเป็นต้องเพิ่มไปยังไซต์อินทราเน็ต</span><span class="sxs-lookup"><span data-stu-id="dbd4f-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="dbd4f-104">ถ้าก่อนหน้านี้ได้ถูกเพิ่มไปยังไซต์ที่เชื่อถือได้และ SSO แบบไม่มีรอยต่อถูกใช้งาน</span><span class="sxs-lookup"><span data-stu-id="dbd4f-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="dbd4f-105">โปรดตรวจสอบ[รายการตรวจสอบการแก้ปัญหา SSO ที่ไร้รอยต่อ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)</span><span class="sxs-lookup"><span data-stu-id="dbd4f-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="dbd4f-106">ทําตามขั้นตอนเหล่านี้เพื่อเพิ่ม URL ลงในรายการไซต์อินทราเน็ต:</span><span class="sxs-lookup"><span data-stu-id="dbd4f-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="dbd4f-107">เปิด Internet Explorer ด้วยการคลิกปุ่ม**เริ่ม**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="dbd4f-108">ในกล่องค้นหา ให้พิมพ์ Internet Explorer จากนั้นในรายการผลลัพธ์ ให้คลิก**Internet Explorer**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="dbd4f-109">คลิก**เครื่องมือ**แล้วคลิก**ตัวเลือกอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="dbd4f-110">คลิกการ**การรักษาความปลอดภัย**แท็บ</span><span class="sxs-lookup"><span data-stu-id="dbd4f-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="dbd4f-111">ตอนนี้คลิกที่**เว็บไซต์อินทราเน็ตท้องถิ่น**แล้วคลิกที่ปุ่ม**เว็บไซต์**แล้วปุ่ม**ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="dbd4f-112">ป้อน URL ของเว็บไซต์ และคลิก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="dbd4f-113">เมื่อคุณดําเนินการเสร็จสิ้นแล้ว ให้คลิก**ปิด**</span><span class="sxs-lookup"><span data-stu-id="dbd4f-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="dbd4f-114">สําหรับข้อมูลเพิ่มเติม ให้ดู[เอกสารประกอบสําหรับการปรับใช้ SSO แบบไม่มีรอยต่อสําหรับ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (รวมถึงกระบวนการตามนโยบายเพื่อเพิ่ม URL ไปยังไซต์อินทราเน็ตในขั้นตอนที่ 3)</span><span class="sxs-lookup"><span data-stu-id="dbd4f-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
