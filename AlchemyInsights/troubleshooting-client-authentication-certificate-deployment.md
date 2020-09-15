---
title: การปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659005"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="ba729-102">การปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="ba729-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="ba729-103">โปรแกรม Intune NDES/SCEP และโพรไฟล์ใบรับรองของไคลเอ็นต์แบบ PKCS/PFX จะใช้ร่วมกับชนิดของโปรไฟล์อื่นๆเช่น Wifi, VPN และอีเมลเพื่ออนุญาตให้ผู้ใช้สามารถรับรองความถูกต้องของทรัพยากรขององค์กรได้</span><span class="sxs-lookup"><span data-stu-id="ba729-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="ba729-104">เมื่อชนิดโพรไฟล์เหล่านั้นถูกลิงก์ไปยังโปรไฟล์ใบรับรองไคลเอ็นต์จะขึ้นอยู่กับการปรับใช้ของโพรไฟล์นั้นเสร็จเรียบร้อยแล้ว</span><span class="sxs-lookup"><span data-stu-id="ba729-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="ba729-105">การตั้งค่าโครงสร้างพื้นฐานเริ่มต้นและการกำหนดค่าที่เกี่ยวข้องของโปรไฟล์ใบรับรองไคลเอ็นต์มักจำเป็นต้องมีการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="ba729-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="ba729-106">สำหรับคำแนะนำทีละขั้นตอนในการตั้งค่าที่ประสบความสำเร็จของตัวเชื่อมต่อ NDES และคำแนะนำในการแก้ไขปัญหาเพื่อแยกปัญหาเกี่ยวกับการปรับใช้ใบรับรองให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="ba729-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="ba729-107">กำหนดค่าโครงสร้างพื้นฐานเพื่อสนับสนุน SCEP ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="ba729-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="ba729-108">ภาพรวมสำหรับการแก้ไขปัญหาส่วนกำหนดค่า SCEP ที่มี Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ba729-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="ba729-109">ใช้สคริปต์ powershell ที่อ้างอิงเพื่อช่วยในการตรวจสอบการกำหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="ba729-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="ba729-110">สำหรับข้อมูลเพิ่มเติมให้ดูที่สคริปต์การตรวจสอบความถูกต้องของ[ใบรับรองของ Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)</span><span class="sxs-lookup"><span data-stu-id="ba729-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="ba729-111">**ปัญหาทั่วไปอื่นๆ**</span><span class="sxs-lookup"><span data-stu-id="ba729-111">**Other common issues**</span></span>

<span data-ttu-id="ba729-112">**เมื่อฉันพยายามติดตั้งตัวเชื่อมต่อใบรับรอง Intune บนเซิร์ฟเวอร์ตัวเชื่อมต่อ NDES ฉันจะได้รับข้อความ "รหัสผ่านในการร้องขอใบรับรองไม่สามารถตรวจสอบได้ อาจมีการใช้งานแล้ว รับรหัสผ่านใหม่เพื่อส่งพร้อมกับคำขอนี้ "**</span><span class="sxs-lookup"><span data-stu-id="ba729-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="ba729-113">ข้อความนี้หมายความว่าคุณจำเป็นต้องเรียกใช้การติดตั้งตัวเชื่อมต่อใบรับรองในฐานะผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="ba729-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="ba729-114">ในบางสภาพแวดล้อมเซิร์ฟเวอร์ที่การเรียกใช้ใบรับรอง Intune ต้องใช้พร็อกซีเซิร์ฟเวอร์เพื่อเชื่อมต่อกับ Intune และเพื่อให้ตัวเชื่อมต่อใบรับรองต้องใช้พร็อกซี</span><span class="sxs-lookup"><span data-stu-id="ba729-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="ba729-115">ในบางสถานการณ์ตัวเชื่อมต่อ NDES จะละเว้นการตั้งค่าพร็อกซีที่กำหนดค่าไว้แล้วและอาจจำเป็นต้องกำหนดค่าการตั้งค่าพร็อกซีขณะที่ทำงานอยู่ในบริบทการรักษาความปลอดภัยของ LocalSystem</span><span class="sxs-lookup"><span data-stu-id="ba729-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="ba729-116">วิธีแก้ไขคือการเรียกใช้ Internet Explorer เป็นระบบและกำหนดค่าพร็อกซีใน IE</span><span class="sxs-lookup"><span data-stu-id="ba729-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="ba729-117">หลังจากรีสตาร์ทครั้งของบริการตัวเชื่อมต่อ Intune ตัวเชื่อมต่อ NDES จะเชื่อมต่อกับ Intune</span><span class="sxs-lookup"><span data-stu-id="ba729-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="ba729-118">**อุปกรณ์ของผู้ใช้ไม่ได้รับใบรับรอง SCEP จาก NDES อีกต่อไป**</span><span class="sxs-lookup"><span data-stu-id="ba729-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="ba729-119">อาจเป็นไปได้ว่าใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ออกให้กับเซิร์ฟเวอร์ NDES และระบุไว้ในระหว่างการติดตั้งตัวเชื่อมต่อ NDES หมดอายุหรือหายไป</span><span class="sxs-lookup"><span data-stu-id="ba729-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="ba729-120">เมื่อต้องการแก้ไข:</span><span class="sxs-lookup"><span data-stu-id="ba729-120">To resolve:</span></span> 
 
1. <span data-ttu-id="ba729-121">ถอนการติดตั้งตัวเชื่อมต่อ NDES</span><span class="sxs-lookup"><span data-stu-id="ba729-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="ba729-122">ใช้รายละเอียดเหล่านี้เพื่อร้องขอการรับรองความถูกต้องของไคลเอ็นต์ใหม่หรือใบรับรองการรับรองความถูกต้องของเซิร์ฟเวอร์:</span><span class="sxs-lookup"><span data-stu-id="ba729-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="ba729-123">ชื่อเรื่อง: CN = fqdn ภายนอก</span><span class="sxs-lookup"><span data-stu-id="ba729-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="ba729-124">ชื่อสำรองของชื่อเรื่อง (จำเป็นต้องใช้ทั้งสองอย่าง): DNS = fqdn ภายนอก DNS = fqdn ภายใน</span><span class="sxs-lookup"><span data-stu-id="ba729-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="ba729-125">ติดตั้งตัวเชื่อมต่อ NDES ใหม่ด้วยใบรับรองใหม่</span><span class="sxs-lookup"><span data-stu-id="ba729-125">Reinstall the NDES connector with the new certificate.</span></span>