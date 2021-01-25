---
title: ปัญหาเกี่ยวกับลิงก์และ Url
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974756"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="1c57a-102">ปัญหาเกี่ยวกับลิงก์และ Url</span><span class="sxs-lookup"><span data-stu-id="1c57a-102">Issues with links and URLs</span></span>

<span data-ttu-id="1c57a-103">การเปลี่ยนเส้นทาง Url URI/ตอบกลับ (ทั้งสองนิพจน์จะสามารถเปลี่ยนได้) คือ Url ที่ใช้โดยแพลตฟอร์มสำหรับข้อมูลเฉพาะตัวของ Microsoft เพื่อส่งกลับโทเค็นที่ร้องขอแอป</span><span class="sxs-lookup"><span data-stu-id="1c57a-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="1c57a-104">สำหรับข้อมูลเกี่ยวกับ Url เหล่านี้ให้ดูบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1c57a-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="1c57a-105">[ขั้นตอนการรับรองความถูกต้องและสถานการณ์สมมติของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -ข้อมูลเกี่ยวกับการเปลี่ยนเส้นทาง URIs ในหน้าการ **ลงทะเบียนแอปของ** แต่ละสถานการณ์</span><span class="sxs-lookup"><span data-stu-id="1c57a-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="1c57a-106">การเปลี่ยนเส้นทางข้อจำกัดและข้อจำกัดของ URL ของ URI/ตอบกลับ</span><span class="sxs-lookup"><span data-stu-id="1c57a-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="1c57a-107">**ฉันไม่ทราบวิธีการลงทะเบียน URL URI/ตอบกลับที่ถูกเปลี่ยนเส้นทางขวาสำหรับแอปของฉัน**</span><span class="sxs-lookup"><span data-stu-id="1c57a-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="1c57a-108">เมื่อคุณลงชื่อเข้าใช้ด้วยแอปพลิเคชันที่คุณกำลังพัฒนาถ้ากล่องโต้ตอบการลงชื่อเข้าใช้แสดง **AADSTS50011: url ตอบกลับที่ระบุในการร้องขอไม่ตรง <your app ID> กับ url ตอบกลับที่กำหนดค่าไว้สำหรับแอปพลิเคชัน** คุณจะต้องเพิ่มลงในการลงทะเบียนแอปพลิเคชันของคุณ, URI การเปลี่ยนเส้นทางที่รหัสของคุณใช้ในการร้องขอโท</span><span class="sxs-lookup"><span data-stu-id="1c57a-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="1c57a-109">เมื่อต้องการเพิ่ม URL การตอบกลับให้ไปที่แท็บการ **รับรองความถูกต้อง** ในหน้าการ **ลงทะเบียนแอปพลิเคชัน** ของคุณในพอร์ทัล Azure และเพิ่มรายการในส่วนการ **เปลี่ยนเส้นทาง URIs**</span><span class="sxs-lookup"><span data-stu-id="1c57a-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="1c57a-110">เปลี่ยนเส้นทาง URIs จะถูกพิมพ์ (เว็บหรืออุปกรณ์เคลื่อนที่/เดสก์ท็อป)</span><span class="sxs-lookup"><span data-stu-id="1c57a-110">Redirect URIs are typed (Web or mobile/desktop).</span></span> <span data-ttu-id="1c57a-111">ค่าที่คุณจำเป็นต้องใส่จะขึ้นอยู่กับชนิดของแอปพลิเคชันที่คุณกำลังสร้างตามที่อธิบายไว้ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="1c57a-111">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="1c57a-112">สำหรับแอปพลิเคชันหน้าเดียวและเว็บแอป URL ตอบกลับคือ URL ในแอปพลิเคชันของคุณ</span><span class="sxs-lookup"><span data-stu-id="1c57a-112">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="1c57a-113">ดูการ [ลงทะเบียนแอปพลิเคชันหน้าเดียว](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) หรือ [ลงทะเบียนแอป web App โดยใช้ Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="1c57a-113">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="1c57a-114">สำหรับแอปเดสก์ท็อปค่าที่คุณจำเป็นต้องเลือกจะขึ้นอยู่กับ:</span><span class="sxs-lookup"><span data-stu-id="1c57a-114">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="1c57a-115">platform (MacOS จะแตกต่างจาก Windows หรือ Linux)</span><span class="sxs-lookup"><span data-stu-id="1c57a-115">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="1c57a-116">วิธีที่คุณได้รับโทเค็น (แบบโต้ตอบที่มีการทำงานของรหัสอุปกรณ์ที่มีการรับรองความถูกต้องของ Windows แบบรวม [IWA] หรือที่มีชื่อผู้ใช้/รหัสผ่าน)</span><span class="sxs-lookup"><span data-stu-id="1c57a-116">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="1c57a-117">สำหรับรายละเอียดให้ดูที่การ [ลงทะเบียนแอปบนเดสก์ท็อป-การเปลี่ยนเส้นทาง URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="1c57a-117">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="1c57a-118">สำหรับแอปพลิเคชันมือถือ URI การเปลี่ยนเส้นทางจะขึ้นอยู่กับ:</span><span class="sxs-lookup"><span data-stu-id="1c57a-118">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="1c57a-119">platform (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="1c57a-119">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="1c57a-120">ข้อมูลที่ใช้ในการสร้างแอปของคุณเช่น ID bundle ใน iOS และชื่อแพคเกจและการแฮชสำหรับลายเซ็นบน Android การลงทะเบียนแอป Azure portal จะช่วยคุณได้</span><span class="sxs-lookup"><span data-stu-id="1c57a-120">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="1c57a-121">สำหรับรายละเอียดให้ดูที่[การกำหนดค่าของแพลตฟอร์มและการเปลี่ยนเส้นทาง URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="1c57a-121">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="1c57a-122">เว็บ APIs และบางวิธีที่เงียบของการรับโทเค็น (IWA และชื่อผู้ใช้/รหัสผ่าน) ไม่จำเป็นต้องมี URI การเปลี่ยนเส้นทาง</span><span class="sxs-lookup"><span data-stu-id="1c57a-122">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="1c57a-123">**ฉันได้ปรับใช้แอปพลิเคชันเว็บของฉันและเมื่อฉันทดสอบแอปที่ปรับใช้แล้วฉันจะได้รับข้อความตอบกลับ url ที่ไม่ตรงกัน**</span><span class="sxs-lookup"><span data-stu-id="1c57a-123">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="1c57a-124">เพิ่มการเปลี่ยนเส้นทาง URIs สำหรับตำแหน่งที่ตั้งทั้งหมดที่คุณกำลังปรับใช้แอปพลิเคชันบนเว็บของคุณ</span><span class="sxs-lookup"><span data-stu-id="1c57a-124">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="1c57a-125">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ลงทะเบียนแอป web app โดยใช้ Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)</span><span class="sxs-lookup"><span data-stu-id="1c57a-125">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="1c57a-126">เพิ่มการเปลี่ยนเส้นทาง URI สำหรับตำแหน่งที่ตั้งทันทีหลังจากที่คุณได้ปรับใช้แอปพลิเคชันที่ตำแหน่งที่ตั้งนั้น</span><span class="sxs-lookup"><span data-stu-id="1c57a-126">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="1c57a-127">**ฉันไม่สามารถลงทะเบียน Url การตอบกลับเพียงพอ**</span><span class="sxs-lookup"><span data-stu-id="1c57a-127">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="1c57a-128">คุณเป็น ISV และมีการเปลี่ยนเส้นทาง URIs หนึ่งหรือหลายรายการสำหรับลูกค้าทุกรายของคุณ</span><span class="sxs-lookup"><span data-stu-id="1c57a-128">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="1c57a-129">คุณต้องการโยกย้ายจาก ADAL/Azure AD v1.0 เป็น MSAL/Microsoft identity platform และคุณจะกด[จำนวนสูงสุดของการเปลี่ยนเส้นทาง URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="1c57a-129">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="1c57a-130">เมื่อต้องการแก้ไขปัญหานี้ให้ [เพิ่มการเปลี่ยนเส้นทาง URIs ไปยัง](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) การรักษาบริการที่สอดคล้องกับลูกค้าแต่ละรายของคุณ</span><span class="sxs-lookup"><span data-stu-id="1c57a-130">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
