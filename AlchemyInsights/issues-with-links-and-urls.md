---
title: ปัญหาเกี่ยวกับลิงก์และ URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707901"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="f2ed4-102">ปัญหาเกี่ยวกับลิงก์และ URL</span><span class="sxs-lookup"><span data-stu-id="f2ed4-102">Issues with links and URLs</span></span>

<span data-ttu-id="f2ed4-103">URL การเปลี่ยนเส้นทาง URI/การตอบกลับ (ทั้งสองนิพจน์สามารถสลับกันได้) คือ URL ที่ใช้โดยแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft เพื่อส่งกลับโทเค็นที่ร้องขอโดยแอป</span><span class="sxs-lookup"><span data-stu-id="f2ed4-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="f2ed4-104">ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับ URL เหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="f2ed4-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="f2ed4-105">[การรับรองความถูกต้องโฟลว์และสถานการณ์สมมติ](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) ของแอปพลิเคชัน - ข้อมูลเกี่ยวกับ URI การเปลี่ยนเส้นทาง **ในหน้าการลงทะเบียน** แอปของแต่ละสถานการณ์</span><span class="sxs-lookup"><span data-stu-id="f2ed4-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="f2ed4-106">การเปลี่ยนเส้นทางข้อจํากัดและข้อจํากัดของ URL URI/การตอบกลับ</span><span class="sxs-lookup"><span data-stu-id="f2ed4-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="f2ed4-107">**ฉันไม่ทราบวิธีการลงทะเบียน URI เปลี่ยนเส้นทางที่ถูกต้อง / URL ตอบกลับของแอปของฉัน**</span><span class="sxs-lookup"><span data-stu-id="f2ed4-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="f2ed4-108">เมื่อคุณลงชื่อเข้าใช้ด้วยแอปพลิเคชันที่คุณพัฒนา ถ้ากล่องโต้ตอบลงชื่อเข้าใช้แสดง **AADSTS50011: URL <your app ID>** ตอบกลับที่ระบุในการร้องขอไม่ตรงกับ URL ตอบกลับที่กําหนดค่าไว้ให้กับแอปพลิเคชัน คุณจะต้องเพิ่มไปยังการลงทะเบียนแอปพลิเคชันของคุณ การเปลี่ยนเส้นทาง URI ที่โค้ดของคุณใช้ในการร้องขอโทเค็นไปยังแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="f2ed4-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="f2ed4-109">เมื่อต้องการเพิ่ม URL ตอบกลับ ให้ไปที่แท็บ **การรับรองความถูก\*\*\*\*ต้องในหน้าการลงทะเบียน** แอปพลิเคชันในพอร์ทัล Azure และเพิ่มรายการในส่วน **URI การ** เปลี่ยนเส้นทาง</span><span class="sxs-lookup"><span data-stu-id="f2ed4-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="f2ed4-110">ค่าที่คุณต้องใส่จะขึ้นอยู่กับชนิดของแอปพลิเคชันที่คุณสร้าง ตามที่อธิบายไว้ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="f2ed4-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="f2ed4-111">For single-page applications and web apps, the reply URL is a URL in your application.</span><span class="sxs-lookup"><span data-stu-id="f2ed4-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="f2ed4-112">ดู [การลงทะเบียนแอปพลิเคชันหน้าเดียว](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) หรือ [ลงทะเบียนแอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="f2ed4-113">ในแอปบนเดสก์ท็อป ค่าที่คุณต้องเลือกจะขึ้นอยู่กับสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="f2ed4-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="f2ed4-114">แพลตฟอร์ม (MacOS แตกต่างจาก Windows หรือ Linux)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="f2ed4-115">วิธีที่คุณรับโทเค็น (แบบโต้ตอบด้วยลโฟลว์รหัสอุปกรณ์ด้วยการรับรองความถูกต้องของ Windows แบบรวม [IWA] หรือด้วยชื่อผู้ใช้/รหัสผ่าน)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="f2ed4-116">For details, see [Desktop apps - การลงทะเบียนแอป - เปลี่ยนเส้นทาง URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="f2ed4-117">For mobile applications, the redirect URI depends on:</span><span class="sxs-lookup"><span data-stu-id="f2ed4-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="f2ed4-118">แพลตฟอร์ม (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="f2ed4-119">ข้อมูลที่ใช้ในการสร้างแอปของคุณ เช่น Bundle ID ใน iOS และชื่อแพคเกจและแฮชลายเซ็นบน Android การลงทะเบียนแอปพอร์ทัล Azure จะช่วยคุณได้</span><span class="sxs-lookup"><span data-stu-id="f2ed4-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="f2ed4-120">For details, see [platform configuration and redirect URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="f2ed4-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="f2ed4-121">API เว็บและวิธีที่เงียบบางวิธีในการรับโทเค็น (IWA และชื่อผู้ใช้/รหัสผ่าน) ไม่ต้องมี URI การเปลี่ยนเส้นทาง</span><span class="sxs-lookup"><span data-stu-id="f2ed4-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="f2ed4-122">**ฉันได้ปรับใช้แอปพลิเคชันบนเว็บของฉันและเมื่อฉันทดสอบแอปที่ปรับใช้ ฉันได้รับข้อความตอบกลับ URL ที่ไม่ตรงกัน**</span><span class="sxs-lookup"><span data-stu-id="f2ed4-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="f2ed4-123">เพิ่ม URI เปลี่ยนเส้นทางของทุกที่ตั้งที่คุณปรับใช้แอปพลิเคชันบนเว็บของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2ed4-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="f2ed4-124">ดูข้อมูลเพิ่มเติมในการลงทะเบียน[แอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="f2ed4-125">เพิ่ม URI เปลี่ยนเส้นทางไปยังสถานที่หนึ่งทันทีหลังจากที่คุณได้ปรับใช้แอปพลิเคชันที่สถานที่นั้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="f2ed4-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="f2ed4-126">**ฉันไม่สามารถลงทะเบียน URL ตอบกลับได้มากพอ**</span><span class="sxs-lookup"><span data-stu-id="f2ed4-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="f2ed4-127">คุณเป็น ISV และมี URI เปลี่ยนเส้นทางหนึ่งหรือหลายรายการกับลูกค้าของคุณทุกคน</span><span class="sxs-lookup"><span data-stu-id="f2ed4-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="f2ed4-128">คุณต้องการโยกย้ายจาก ADAL/Azure AD v1.0 ไปยัง MSAL/แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และคุณมีจํานวนสูงสุดในการเปลี่ยนเส้นทาง[URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="f2ed4-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="f2ed4-129">เมื่อต้องการแก้ไขปัญหานี้ [ให้เพิ่ม URI เปลี่ยนเส้นทางไปยังบริการ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) หลักที่สอดคล้องกับลูกค้าของคุณแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="f2ed4-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
