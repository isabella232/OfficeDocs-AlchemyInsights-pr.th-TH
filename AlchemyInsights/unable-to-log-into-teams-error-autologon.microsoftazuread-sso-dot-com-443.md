---
title: ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799979"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="eab79-102">ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon microsoftazuread-sso dot com: 443</span><span class="sxs-lookup"><span data-stu-id="eab79-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="eab79-103">ถ้ามีการเปิดใช้งาน SSO อย่างราบรื่นเป็นการรับรองความถูกต้องของ O365 URL "autologon.microsoftazuread-sso.com" อาจจำเป็นต้องเพิ่มลงในอินทราเน็ตไซต์</span><span class="sxs-lookup"><span data-stu-id="eab79-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="eab79-104">ถ้ามีการเพิ่มไปยังไซต์ที่เชื่อถือได้ก่อนหน้านี้และ SSO ที่ราบรื่นถูกใช้งานอยู่จะถูกเอาออกจากไซต์ที่เชื่อถือได้</span><span class="sxs-lookup"><span data-stu-id="eab79-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="eab79-105">โปรดตรวจทาน[รายการตรวจสอบการแก้ไขปัญหาของ SSO ที่ราบรื่น](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)</span><span class="sxs-lookup"><span data-stu-id="eab79-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="eab79-106">ทำตามขั้นตอนต่อไปนี้เพื่อเพิ่ม URL ลงในรายการไซต์อินทราเน็ต:</span><span class="sxs-lookup"><span data-stu-id="eab79-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="eab79-107">เปิด Internet Explorer ด้วยการคลิกปุ่ม**เริ่ม**</span><span class="sxs-lookup"><span data-stu-id="eab79-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="eab79-108">ในกล่องค้นหาให้พิมพ์ Internet Explorer จากนั้นในรายการผลลัพธ์ให้คลิก**Internet Explorer**</span><span class="sxs-lookup"><span data-stu-id="eab79-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="eab79-109">คลิก**เครื่องมือ**แล้วคลิก**ตัวเลือกอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="eab79-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="eab79-110">คลิกแท็บ**ความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="eab79-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="eab79-111">ในตอนนี้ให้คลิกที่**ไซต์อินทราเน็ตเฉพาะ**ที่จากนั้นคลิกที่ปุ่ม**ไซต์**แล้วกดปุ่ม**ขั้นสูง**</span><span class="sxs-lookup"><span data-stu-id="eab79-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="eab79-112">ใส่ URL ของเว็บไซต์แล้วคลิก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="eab79-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="eab79-113">เมื่อคุณดำเนินการเสร็จสิ้นแล้วให้คลิก**ปิด**</span><span class="sxs-lookup"><span data-stu-id="eab79-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="eab79-114">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [เอกสารประกอบสำหรับการปรับใช้ SSO อย่างราบรื่นสำหรับ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (รวมถึงกระบวนการที่ใช้นโยบายเพื่อเพิ่ม URL ลงในไซต์อินทราเน็ตในขั้นตอนที่ 3)</span><span class="sxs-lookup"><span data-stu-id="eab79-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
