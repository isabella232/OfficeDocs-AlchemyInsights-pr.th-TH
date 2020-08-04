---
title: การแก้ไขปัญหาการปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555807"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="69d4d-102">การแก้ไขปัญหาการปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="69d4d-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="69d4d-103">โปรไฟล์ใบรับรองลูกค้า Intunes NDES/ SCEP และ PKCS/PFX มักใช้ร่วมกับโปรไฟล์ประเภทอื่น ๆ เช่น Wifi, VPN และอีเมลเพื่อให้ผู้ใช้สามารถตรวจสอบสิทธิ์ไปยังทรัพยากรขององค์กรได้</span><span class="sxs-lookup"><span data-stu-id="69d4d-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="69d4d-104">เมื่อชนิดโพรไฟล์เหล่านั้นถูกเชื่อมโยงกับส่วนกําหนดค่าใบรับรองไคลเอ็นต์จะขึ้นอยู่กับการปรับใช้ส่วนกําหนดค่าที่ประสบความสําเร็จ</span><span class="sxs-lookup"><span data-stu-id="69d4d-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="69d4d-105">การตั้งค่าโครงสร้างพื้นฐานเริ่มต้นและการกําหนดค่าที่เกี่ยวข้องของส่วนกําหนดค่าใบรับรองไคลเอ็นต์มักต้องการการแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="69d4d-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="69d4d-106">สําหรับคําแนะนําทีละขั้นตอนการตั้งค่าตัวเชื่อมต่อ NDES ที่สําเร็จ และคําแนะนําในการแก้ไขปัญหาเพื่อแยกปัญหาเกี่ยวกับการปรับใช้ใบรับรอง ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="69d4d-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="69d4d-107">กําหนดค่าโครงสร้างพื้นฐานเพื่อสนับสนุน SCEP ด้วย Intun</span><span class="sxs-lookup"><span data-stu-id="69d4d-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="69d4d-108">ภาพรวมสําหรับการแก้ไขปัญหาโพรไฟล์ใบรับรอง SCEP กับ Microsoft Intun</span><span class="sxs-lookup"><span data-stu-id="69d4d-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="69d4d-109">ใช้สคริปต์ PowerShell อ้างอิงเพื่อช่วยในการตรวจสอบการกําหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="69d4d-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="69d4d-110">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สคริปต์การตรวจสอบตัวเชื่อมต่อ Intunณี Certificate](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)</span><span class="sxs-lookup"><span data-stu-id="69d4d-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="69d4d-111">**ปัญหาทั่วไปอื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="69d4d-111">**Other common issues**</span></span>

<span data-ttu-id="69d4d-112">**เมื่อฉันพยายามที่จะติดตั้งตัวเชื่อมต่อใบรับรอง Intund บนเซิร์ฟเวอร์ตัวเชื่อมต่อ NDES ฉันได้รับข้อความ "รหัสผ่านในการร้องขอใบรับรองไม่สามารถตรวจสอบ มันอาจจะถูกใช้แล้ว ขอรับรหัสผ่านใหม่เพื่อส่งคําขอนี้"**</span><span class="sxs-lookup"><span data-stu-id="69d4d-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="69d4d-113">ข้อความนี้หมายความว่า คุณจําเป็นต้องเรียกใช้การติดตั้งตัวเชื่อมต่อใบรับรองในฐานะผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="69d4d-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="69d4d-114">ในบางสภาพแวดล้อม เซิร์ฟเวอร์ที่ Intuny Certificate รันต้องใช้พร็อกซีเซิร์ฟเวอร์เพื่อเชื่อมต่อกับ Intun ณี และดังนั้นตัวเชื่อมต่อใบรับรองต้องใช้พร็อกซี</span><span class="sxs-lookup"><span data-stu-id="69d4d-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="69d4d-115">ในบางสถานการณ์ ตัวเชื่อมต่อ NDES ละเว้นการตั้งค่าพร็อกซีที่กําหนดค่า ไว้ และอาจจําเป็นต้องกําหนดค่าการตั้งค่าพร็อกซีขณะทํางานในบริบทความปลอดภัยของ LocalSystem</span><span class="sxs-lookup"><span data-stu-id="69d4d-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="69d4d-116">โซลูชันคือการเรียกใช้ Internet Explorer เป็นระบบ และกําหนดค่าพร็อกซีใน IE</span><span class="sxs-lookup"><span data-stu-id="69d4d-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="69d4d-117">หลังจากเริ่มการทํางานของบริการตัวเชื่อมต่อ Intun</span><span class="sxs-lookup"><span data-stu-id="69d4d-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="69d4d-118">**อุปกรณ์ของผู้ใช้จะไม่ได้รับใบรับรอง SCEP จาก NDES อีกต่อไป**</span><span class="sxs-lookup"><span data-stu-id="69d4d-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="69d4d-119">เป็นไปได้ว่า ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ออกไปยังเซิร์ฟเวอร์ NDES และระบุในระหว่างการติดตั้งตัวเชื่อมต่อ NDES หมดอายุหรือหายไป</span><span class="sxs-lookup"><span data-stu-id="69d4d-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="69d4d-120">เมื่อต้องการแก้ไข:</span><span class="sxs-lookup"><span data-stu-id="69d4d-120">To resolve:</span></span> 
 
1. <span data-ttu-id="69d4d-121">ถอนการติดตั้งตัวเชื่อมต่อ NDES</span><span class="sxs-lookup"><span data-stu-id="69d4d-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="69d4d-122">ใช้รายละเอียดเหล่านี้เพื่อร้องขอการรับรองความถูกต้องของไคลเอ็นต์ใหม่หรือใบรับรองการรับรองความถูกต้องของเซิร์ฟเวอร์:</span><span class="sxs-lookup"><span data-stu-id="69d4d-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="69d4d-123">ชื่อเรื่อง: CN =fqdn ภายนอก</span><span class="sxs-lookup"><span data-stu-id="69d4d-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="69d4d-124">ชื่ออื่นของชื่อเรื่อง (ทั้งสองต้อง): DNS = fqdn ภายนอก DNS = fqdn ภายใน</span><span class="sxs-lookup"><span data-stu-id="69d4d-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="69d4d-125">ติดตั้งตัวเชื่อมต่อ NDES ด้วยใบรับรองใหม่</span><span class="sxs-lookup"><span data-stu-id="69d4d-125">Reinstall the NDES connector with the new certificate.</span></span>