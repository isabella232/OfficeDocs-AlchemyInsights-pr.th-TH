---
title: ปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปภายในองค์กรของฉัน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868769"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="ceefb-102">ปัญหาเกี่ยวกับการรวม SSO อย่างราบรื่นกับแอปภายในองค์กรของฉัน</span><span class="sxs-lookup"><span data-stu-id="ceefb-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="ceefb-103">เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการรวม SSO ที่ไม่ราบรื่นกับแอปพลิเคชันภายในองค์กรให้ทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ceefb-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="ceefb-104">**ขั้นตอนที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="ceefb-104">**Recommended steps**</span></span>

1. <span data-ttu-id="ceefb-105">เมื่อต้องการกำหนดค่า **แอปพลิเคชันภายในองค์กร** สำหรับการ **ลงชื่อเข้าใช้ครั้งเดียวผ่านทางพร็อกซีแอปพลิเคชัน** ให้ดู [รหัสผ่านลิ่วสำหรับการลงชื่อเข้าใช้ครั้งเดียวด้วยพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)</span><span class="sxs-lookup"><span data-stu-id="ceefb-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="ceefb-106">**การแก้ไขปัญหาเกี่ยวกับพร็อกซีของแอปพลิเคชัน**: เราขอแนะนำให้คุณเริ่มต้นด้วยการตรวจทานการแก้ไขปัญหาการแก้ไขปัญหาการ [เชื่อมต่อพร็อกซีของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)การตรวจสอบความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="ceefb-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="ceefb-107">ถ้าคุณยังคงมีปัญหาในการเชื่อมต่อกับแอปพลิเคชันให้ทำตามขั้นตอนการแก้ไขปัญหาในการ [แก้ปัญหาแอปพลิเคชันพร็อกซีของแอปพลิเค](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)ชัน</span><span class="sxs-lookup"><span data-stu-id="ceefb-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="ceefb-108">คุณสามารถ [ระบุปัญหา CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ได้โดยใช้เครื่องมือตรวจแก้จุดบกพร่องของเบราว์เซอร์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ceefb-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="ceefb-109">เปิดใช้งานเบราว์เซอร์แล้วเรียกดูเว็บแอป</span><span class="sxs-lookup"><span data-stu-id="ceefb-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="ceefb-110">กด **F12** เพื่อเปิดคอนโซลการตรวจแก้จุดบกพร่อง</span><span class="sxs-lookup"><span data-stu-id="ceefb-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="ceefb-111">ลองสร้างทรานแซคชันใหม่และรีวิวข้อความของคอนโซล</span><span class="sxs-lookup"><span data-stu-id="ceefb-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="ceefb-112">การละเมิด CORS สร้างข้อผิดพลาดของคอนโซลเกี่ยวกับจุดเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="ceefb-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="ceefb-113">ปัญหา CORS บางอย่างไม่สามารถแก้ไขได้เช่นเมื่อแอปของคุณเปลี่ยนเส้นทางไปยัง login.microsoftonline.com เพื่อรับรองความถูกต้องและโทเค็นการเข้าถึงหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="ceefb-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="ceefb-114">การโทร CORS จะล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="ceefb-114">The CORS call then fails.</span></span> <span data-ttu-id="ceefb-115">วิธีแก้ไขปัญหาชั่วคราวสำหรับสถานการณ์สมมตินี้คือการขยายอายุการใช้งานของโทเค็นการเข้าถึงเพื่อป้องกันไม่ให้มีการหมดอายุระหว่างเซสชันของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="ceefb-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="ceefb-116">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการทำสิ่งนี้ให้ดูที่ค่าที่ได้จากการกำหนดค่าของ[โทเค็นใน Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="ceefb-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="ceefb-117">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="ceefb-117">**Recommended documents**</span></span>

- [<span data-ttu-id="ceefb-118">วิธีการกำหนดค่าการลงชื่อเข้าระบบครั้งเดียวไปยังแอปพลิเคชันพร็อกซีของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="ceefb-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="ceefb-119">การลงชื่อเข้าใช้ครั้งเดียวของ SAML สำหรับแอปพลิเคชันภายในองค์กรที่มีพร็อกซีแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="ceefb-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="ceefb-120">ทำความเข้าใจและแก้ไขปัญหาพร็อกซีแอปพลิเคชัน active Directory ของ Azure CORS</span><span class="sxs-lookup"><span data-stu-id="ceefb-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="ceefb-121">แก้ไขปัญหาการกำหนดค่าการมอบหมาย Kerberos ที่จำกัดสำหรับพร็อกซีแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="ceefb-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)