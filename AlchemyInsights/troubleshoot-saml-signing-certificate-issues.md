---
title: แก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694452"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="9a540-102">แก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML</span><span class="sxs-lookup"><span data-stu-id="9a540-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="9a540-103">เมื่อต้องการแก้ไขปัญหาใบรับรองการเซ็นชื่อ SAML ให้ปฏิบัติตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="9a540-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="9a540-104">เมื่อคุณเพิ่มแอปพลิเคชันขององค์กรที่สนับสนุน SSO แล้ว Azure จะสร้างใบรับรองที่เรียกว่าใบรับรอง[การเซ็นชื่อ SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="9a540-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="9a540-105">ใบรับรองนี้มีวันหมดอายุ 3 ปี</span><span class="sxs-lookup"><span data-stu-id="9a540-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="9a540-106">เมื่อต้องการเปลี่ยนวันหมดอายุของใบรับรองของคุณ ให้ดู [ปรับแต่งวันหมดอายุของใบรับรองการติดต่อกับภายนอกของคุณ และย้อนกลับไปยังใบรับรอง](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)ใหม่</span><span class="sxs-lookup"><span data-stu-id="9a540-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="9a540-107">Azure จะใช้ใบรับรองนี้ในการเซ็นชื่อโทเค็น SAML ที่ร้องขอโดยแอปพลิเคชันและส่งไปยังแอปพลิเคชันเพื่อให้ SSO ประสบความสําเร็จ</span><span class="sxs-lookup"><span data-stu-id="9a540-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="9a540-108">เมื่อต้องการเสร็จสิ้น ให้ดาวน์โหลดใบรับรองจากพอร์ทัล Azure และส่งไปยังผู้ออกแอปพลิเคชันเพื่อเสร็จสิ้นกระบวนการ SSO</span><span class="sxs-lookup"><span data-stu-id="9a540-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="9a540-109">หลังจากกระบวนการนี้เสร็จสมบูรณ์ แอปพลิเคชันของคุณจะเชื่อถือใบรับรองนี้และโทเค็น SAML ทั้งหมดที่เซ็นชื่อโดยใบรับรองนี้จะได้รับการยอมรับจากแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="9a540-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="9a540-110">ถ้าใบรับรองนี้หมดอายุ ให้สร้างใบรับรองใหม่ อัปเดตใบรับรองนั้นไปยังผู้เช่าแอปพลิเคชัน แล้วเปิดใช้งานบนด้าน Azure</span><span class="sxs-lookup"><span data-stu-id="9a540-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="9a540-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="9a540-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="9a540-112">ถ้าใบรับรองหมดอายุ ผู้ใช้จะไม่ถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="9a540-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="9a540-113">[เพิ่มที่อยู่อีเมลเพื่อให้ได้รับ](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) การแจ้งเตือนก่อนที่ใบรับรองปัจจุบันจะหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="9a540-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="9a540-114">ขั้นตอนที่ 4 เป็นตัวเลือกหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="9a540-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="9a540-115">เปลี่ยนตัวเลือกการเซ็นชื่อใบรับรอง SAML ของแอปพลิเคชันและอัลกอริทึมการเซ็นชื่อใบรับรอง</span><span class="sxs-lookup"><span data-stu-id="9a540-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="9a540-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="9a540-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

