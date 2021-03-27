---
title: แนวคิดการรับรองความถูกต้องขั้นสูงที่ใช้กับ Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398604"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="b6caf-102">แนวคิดการรับรองความถูกต้องขั้นสูงที่ใช้กับ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b6caf-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="b6caf-103">ต่อไปนี้คือแนวคิดการรับรองความถูกต้องขั้นสูงที่ใช้กับ Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="b6caf-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="b6caf-104">**การรับรองความถูกต้องแบบโพรแอกทีฟ**</span><span class="sxs-lookup"><span data-stu-id="b6caf-104">**Proactive Authentication**</span></span>

<span data-ttu-id="b6caf-105">เมื่อคุณเปิดใช้งานนโยบาย [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge จะพยายามรับรองความถูกต้องของผู้ใช้ที่ลงชื่อเข้าใช้เชิงรุกผ่านบริการของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="b6caf-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="b6caf-106">ตามช่วงเวลาที่สม่่าเป็น จะใช้บริการออนไลน์เพื่อตรวจสอบรายการที่ถูกอัปเดตซึ่งมีการกําหนดค่าที่ควบคุมการรับรองความถูกต้องแบบโพรแอกทีฟ</span><span class="sxs-lookup"><span data-stu-id="b6caf-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="b6caf-107">สิทธิประโยชน์: การรับรองความถูกต้องแบบโพรแอกทีฟจะเปิดใช้งานการรับรองความถูกต้องกับบริการหลัก เช่น หน้าแท็บใหม่ของ Office</span><span class="sxs-lookup"><span data-stu-id="b6caf-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="b6caf-108">นอกจากนี้ ถ้า Bing ถูกใช้เป็นโปรแกรมค้นหา การรับรองความถูกต้องแบบโพรแอกทีฟจะช่วยปรับปรุงประสิทธิภาพของแถบที่อยู่ และช่วยสร้างผลลัพธ์การค้นหาที่ปรับให้เหมาะกับความต้องการของธุรกิจของคุณ</span><span class="sxs-lookup"><span data-stu-id="b6caf-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="b6caf-109">**การรับรองความถูกต้องของ NTLM ของ Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="b6caf-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="b6caf-110">ถ้าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) ไม่พร้อมใช้งานเมื่อเว็บไซต์พยายามลงชื่อเข้าใช้ผู้ใช้ผ่านกลไก NTLM หรือ Negotiate ฟีเจอร์นี้จะอนุญาตให้ผู้ใช้แชร์ข้อมูลรับรองความถูกต้องของระบบปฏิบัติการกับเว็บไซต์ และเป็นไปตามความท้าทายในการรับรองความถูกต้องโดยใช้ UI ของ Windows Hello Cred</span><span class="sxs-lookup"><span data-stu-id="b6caf-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="b6caf-111">โฟลว์การลงชื่อเข้าใช้นี้จะปรากฏเฉพาะใน Windows 10 และเฉพาะผู้ใช้ที่ไม่ได้รับ SSO ระหว่าง NTLM หรือปัญหา Negotiate เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="b6caf-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="b6caf-112">**ใช้รหัสผ่านที่บันทึกไว้เพื่อลงชื่อเข้าใช้โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="b6caf-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="b6caf-113">ผู้ใช้ที่บันทึกรหัสผ่านใน Microsoft Edge สามารถเปิดใช้งานการเข้าสู่ระบบเว็บไซต์ที่พวกเขาได้บันทึกข้อมูลอ้างอิงโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b6caf-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="b6caf-114">ผู้ใช้สามารถเปิดหรือปิดฟีเจอร์นี้ edge://settings/passwords และคุณสามารถกําหนดค่าในนโยบาย [ตัวจัดการ](https://go.microsoft.com/fwlink/?linkid=2134622) รหัสผ่านได้</span><span class="sxs-lookup"><span data-stu-id="b6caf-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
