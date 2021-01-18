---
title: การกำหนดค่าพร็อกซีของแอป
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885530"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="f1885-102">การกำหนดค่าพร็อกซีของแอป</span><span class="sxs-lookup"><span data-stu-id="f1885-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="f1885-103">เมื่อต้องการทำความเข้าใจเกี่ยวกับวิธีการกำหนดค่าแอปพลิเคชันพร็อกซีของแอปพลิเคชันภายใน Azure AD เพื่อแสดงแอปพลิเคชันภายในองค์กรของคุณไปยัง cloud ให้ดูที่[วิธีการกำหนดค่าแอปพลิเคชันพร็อกซี](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="f1885-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="f1885-104">การลงชื่อเข้าระบบครั้งเดียว (SSO) ช่วยให้ผู้ใช้ของคุณสามารถเข้าถึงแอปพลิเคชันได้โดยไม่มีการรับรองความถูกต้องหลายครั้ง</span><span class="sxs-lookup"><span data-stu-id="f1885-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="f1885-105">จะอนุญาตให้มีการรับรองความถูกต้องเดียวที่จะเกิดขึ้นในระบบคลาวด์จาก Azure Active directory และอนุญาตให้บริการหรือตัวเชื่อมต่อเพื่อ impersonate ผู้ใช้ให้ทำการท้าทายการรับรองความถูกต้องเพิ่มเติมใดๆเพิ่มเติมจากแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="f1885-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="f1885-106">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่ [วิธีการกำหนดค่าการลงชื่อเข้าระบบครั้งเดียวไปยังแอปพลิเคชันพร็อกซีแอปพลิ](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)เคชัน</span><span class="sxs-lookup"><span data-stu-id="f1885-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="f1885-107">ใช้ [บทความนี้](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) เพื่อแก้ไขปัญหาทั่วไปที่คนหน้าเมื่อสร้างแอปพลิเคชันพร็อกซีของแอปพลิเคชันใหม่</span><span class="sxs-lookup"><span data-stu-id="f1885-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="f1885-108">ถ้าคุณกำลังมีปัญหาในการตั้งค่าการรับรองความถูกต้องของการสิ้นสุดหลังไปยังแอปพลิเคชันของคุณคุณอาจต้องการแก้ไขปัญหาการ[กำหนดค่าการมอบสิทธิ์ kerberos ที่จำกัดสำหรับพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to)หรือทำตามคำแนะนำเกี่ยวกับการ[กำหนดค่าแอปพลิเคชันด้วย PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to)</span><span class="sxs-lookup"><span data-stu-id="f1885-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
