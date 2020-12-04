---
title: แนวคิดการรับรองความถูกต้องขั้นสูงที่สามารถใช้ได้กับ Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573779"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="db69c-102">แนวคิดการรับรองความถูกต้องขั้นสูงที่สามารถใช้ได้กับ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="db69c-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="db69c-103">ต่อไปนี้คือแนวคิดการรับรองความถูกต้องขั้นสูงที่สามารถใช้ได้กับ Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="db69c-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="db69c-104">**การรับรองความถูกต้องเชิงรุก**</span><span class="sxs-lookup"><span data-stu-id="db69c-104">**Proactive Authentication**</span></span>

<span data-ttu-id="db69c-105">เมื่อคุณเปิดใช้งานนโยบาย [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge จะพยายามตรวจสอบความถูกต้องของผู้ใช้ที่ลงชื่อเข้าใช้ผ่านทาง microsoft service</span><span class="sxs-lookup"><span data-stu-id="db69c-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="db69c-106">ในช่วงเวลาปกติมันจะใช้บริการออนไลน์เพื่อตรวจสอบรายการที่อัปเดตที่มีการกำหนดค่าที่ควบคุมการรับรองความถูกต้องเชิงรุก</span><span class="sxs-lookup"><span data-stu-id="db69c-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="db69c-107">ประโยชน์: การรับรองความถูกต้องเชิงรุกเปิดใช้งานการรับรองความถูกต้องไปยังบริการหลักๆเช่นหน้าแท็บใหม่ของ Office</span><span class="sxs-lookup"><span data-stu-id="db69c-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="db69c-108">นอกจากนี้ถ้าใช้ Bing เป็นโปรแกรมค้นหาการรับรองความถูกต้องเชิงรุกจะช่วยปรับปรุงประสิทธิภาพการทำงานของแถบที่อยู่และช่วยสร้างผลลัพธ์การค้นหาให้เป็นแบบส่วนตัวตามความต้องการของธุรกิจของคุณ</span><span class="sxs-lookup"><span data-stu-id="db69c-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="db69c-109">**Windows Hello CredUI สำหรับการรับรองความถูกต้องของ NTLM**</span><span class="sxs-lookup"><span data-stu-id="db69c-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="db69c-110">ถ้าการลงชื่อเข้าใช้ครั้งเดียว (SSO) ไม่พร้อมใช้งานเมื่อเว็บไซต์พยายามที่จะลงชื่อเข้าใช้ผู้ใช้ผ่านทางกลไกของ NTLM หรือการเจรจาฟีเจอร์นี้จะอนุญาตให้ผู้ใช้แชร์ข้อมูลประจำตัวของระบบปฏิบัติการกับเว็บไซต์และเพื่อตอบสนองความท้าทายการรับรองความถูกต้องโดยใช้ Windows Hello Cred UI</span><span class="sxs-lookup"><span data-stu-id="db69c-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="db69c-111">ขั้นตอนการลงชื่อเข้าใช้นี้จะปรากฏเฉพาะใน Windows 10 และเฉพาะผู้ใช้ที่ไม่ได้รับ SSO ในระหว่างที่มีความท้าทาย NTLM หรือเจรจาต่อรองเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="db69c-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="db69c-112">**ใช้รหัสผ่านที่บันทึกไว้เพื่อลงชื่อเข้าใช้โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="db69c-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="db69c-113">ผู้ใช้ที่บันทึกรหัสผ่านใน Microsoft Edge สามารถเปิดใช้งานการลงชื่อเข้าใช้โดยอัตโนมัติไปยังเว็บไซต์ที่พวกเขาได้บันทึกข้อมูลประจำตัว</span><span class="sxs-lookup"><span data-stu-id="db69c-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="db69c-114">ผู้ใช้สามารถเปิดหรือปิดฟีเจอร์นี้ใน edge://settings/passwords และคุณสามารถกำหนดค่าได้ในนโยบาย[ตัวจัดการรหัสผ่าน](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="db69c-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
