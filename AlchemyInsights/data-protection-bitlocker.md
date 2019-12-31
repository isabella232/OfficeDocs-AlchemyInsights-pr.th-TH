---
title: การระบุ-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908728"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="58828-102">การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="58828-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="58828-103">สามารถใช้นโยบายการป้องกันปลายทาง Intune เพื่อกำหนดการตั้งค่าการเข้ารหัสลับของ Bitlocker สำหรับอุปกรณ์ Windows</span><span class="sxs-lookup"><span data-stu-id="58828-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="58828-104">สำหรับข้อมูลเพิ่มเติมให้ดู[การตั้งค่า Windows 10 (และรุ่นที่ใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="58828-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="58828-105">คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย Bitlocker โดยอัตโนมัติซึ่งจะถูกทริกเกอร์โดยไม่มีแอพลิเคชันของนโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="58828-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="58828-106">ซึ่งอาจส่งผลกระทบต่อการใช้นโยบายหากการตั้งค่าที่ไม่ใช่แบบเริ่มต้นถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="58828-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="58828-107">ดูคำถามที่พบบ่อยต่อไปนี้สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="58828-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="58828-108">สำหรับข้อมูลเกี่ยวกับการแก้ไขปัญหาเกี่ยวกับ bitlocker โปรดดูที่การ[แก้ไขปัญหานโยบาย bitlocker ใน Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)</span><span class="sxs-lookup"><span data-stu-id="58828-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="58828-109">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="58828-109">**FAQ**</span></span>

 <span data-ttu-id="58828-110">ถาม: Windows รุ่นใดที่สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันปลายทาง</span><span class="sxs-lookup"><span data-stu-id="58828-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="58828-111">A: การตั้งค่าในนโยบายการป้องกันการปลายทาง Intune จะดำเนินการโดยใช้ใน[BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="58828-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="58828-112">รุ่นหรือรุ่นทั้งหมดของ Windows ไม่สนับสนุน Bitlocker CSP</span><span class="sxs-lookup"><span data-stu-id="58828-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="58828-113">ในเวลานี้รุ่น Windows ต่อไปนี้ได้รับการสนับสนุน: องค์กร, การศึกษา, มือถือ, องค์กรมือถือ, และมืออาชีพ (สร้าง๑๘๐๙และรุ่นที่ใหม่กว่า).</span><span class="sxs-lookup"><span data-stu-id="58828-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="58828-114">ถาม: หากอุปกรณ์ถูกเข้ารหัสด้วย Bitlocker อยู่แล้วโดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับวิธีการเข้ารหัสและความแข็งแรงของรหัส (XTS-AES-๑๒๘) จะใช้นโยบายกับการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ด้วยการตั้งค่าใหม่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="58828-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="58828-115">A: ไม่</span><span class="sxs-lookup"><span data-stu-id="58828-115">A: No.</span></span> <span data-ttu-id="58828-116">ในการใช้การตั้งค่าการรหัสใหม่จะต้องถอดรหัสลับไดรฟ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="58828-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="58828-117">**หมายเหตุ:** สำหรับอุปกรณ์ที่มีการลงทะเบียนกับออโตไพลอตการเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นในระหว่าง OOBE จะไม่ทริกเกอร์จนกว่าจะมีการประเมินนโยบาย Intune ซึ่งจะช่วยให้การตั้งค่าตามนโยบายที่จะใช้ในตำแหน่งของค่าเริ่มต้นของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="58828-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="58828-118">ถาม: ถ้าอุปกรณ์ถูกเข้ารหัสเป็นผลมาจากการประยุกต์ใช้นโยบาย Intune จะถูกถอดรหัสลับเมื่อมีการลบนโยบายนั้นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="58828-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="58828-119">A: การเอาออกของนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ส่งผลให้การถอดรหัสลับของไดรฟ์ที่ถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="58828-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="58828-120">ถาม: เหตุใดนโยบายการปฏิบัติตามกฎระเบียบ Intune จึงแสดงว่าอุปกรณ์ของฉันไม่ได้เปิดใช้งาน Bitlocker แม้ว่าจะเป็นอย่างไร</span><span class="sxs-lookup"><span data-stu-id="58828-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="58828-121">A: การตั้งค่า "Bitlocker เปิดใช้งาน" ในนโยบายการปฏิบัติตามกฎระเบียบ Intune ใช้ไคลเอนต์การรับรองความสมบูรณ์ของอุปกรณ์ Windows (DHA)</span><span class="sxs-lookup"><span data-stu-id="58828-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="58828-122">ไคลเอนต์นี้วัดเฉพาะสถานะของอุปกรณ์ในเวลาบูต</span><span class="sxs-lookup"><span data-stu-id="58828-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="58828-123">ดังนั้นถ้าไม่มีการเริ่มระบบของอุปกรณ์อีกครั้งเนื่องจากการเข้ารหัสลับด้วย Bitlocker เสร็จสมบูรณ์แล้วบริการไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ขณะกำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="58828-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 