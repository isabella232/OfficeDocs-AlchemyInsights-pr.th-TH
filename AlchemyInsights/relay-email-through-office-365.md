---
title: ส่งอีเมลผ่านMicrosoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118002"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="20d55-102">ตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="20d55-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="20d55-103">เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกและขั้นตอนของคุณ ให้ดู[วิธีการตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมลโดยใช้](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="20d55-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="20d55-104">ถ้าคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดการใช้งานได้เมื่อเร็วๆ นี้ ปัญหาที่พบบ่อยที่สุดคือ:</span><span class="sxs-lookup"><span data-stu-id="20d55-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="20d55-105">**ข้อผิดพลาดที่เกี่ยวข้องกับการรับรองความถูกต้องขณะใช้การส่งไคลเอ็นต์การรับรองความถูกต้องของ SMTP** เราเพิ่งเปลี่ยนแปลงบางอย่างที่เกี่ยวข้องกับวิธีการใช้งานการรับรองความถูกต้องของ SMTP</span><span class="sxs-lookup"><span data-stu-id="20d55-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="20d55-106">For more information about how to resolve issues, see the authentication unsuessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="20d55-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="20d55-107">**เรายอมรับเฉพาะเวอร์ชัน TLS 1.2 ขณะที่สร้างการเชื่อมต่อที่ปลอดภัยOffice 365** ถ้าคุณใช้การเชื่อมต่อที่ปลอดภัย (TLS) ตรวจสอบให้แน่ใจว่าอุปกรณ์แอปพลิเคชันของคุณสนับสนุน TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="20d55-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="20d55-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="20d55-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="20d55-109">ดูปัญหาและวิธีแก้ปัญหาอื่นๆ[ที่แก้ไขปัญหาเกี่ยวกับเครื่องพิมพ์ สแกนเนอร์](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)และแอปพลิเคชัน LOB ที่ส่งอีเมลโดยใช้Microsoft 365 หรือOffice 365</span><span class="sxs-lookup"><span data-stu-id="20d55-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="20d55-110">เมื่อต้องการดูอุปกรณ์ที่ได้รับผลกระทบ ให้ไปที่รายงาน ไคลเอ็นต์ [การรับรองความถูกต้องของ](https://protection.office.com/mailflow/dashboard)SMTP</span><span class="sxs-lookup"><span data-stu-id="20d55-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="20d55-111">**หมายเหตุ**: Exchange Onlineสถานการณ์การส่งจดหมายเป็นกลุ่มไม่ได้</span><span class="sxs-lookup"><span data-stu-id="20d55-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="20d55-112">เมื่อต้องการส่งอีเมลเชิงพาณิชย์เป็นกลุ่ม (ตัวอย่างเช่น จดหมายข่าวของลูกค้า) คุณควรใช้ผู้ให้บริการของบริษัทอื่นที่มีข้อมูลไม่มากในบริการเหล่านี้</span><span class="sxs-lookup"><span data-stu-id="20d55-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
