---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815634"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="8bbbe-102">การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intun1</span><span class="sxs-lookup"><span data-stu-id="8bbbe-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="8bbbe-103">นโยบายการป้องกันปลายทางของ Intunes สามารถใช้เพื่อกําหนดค่าการตั้งค่าการเข้ารหัสลับ Bitlocker บนอุปกรณ์ Windows</span><span class="sxs-lookup"><span data-stu-id="8bbbe-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="8bbbe-104">หากต้องการข้อมูลเพิ่มเติม โปรดดูการตั้งค่า[Windows 10 (และใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intun1](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="8bbbe-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="8bbbe-105">นอกจากนโยบายการป้องกันจุดสิ้นสุดแล้ว ยังมีรายงานการเข้ารหัสลับซึ่งให้มุมมองโดยละเอียดมากขึ้นของสถานะการเข้ารหัสลับของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="8bbbe-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="8bbbe-106">รายงานนี้สามารถเข้าถึงได้จากพอร์ทัล MEM ภายใต้ **อุปกรณ์ > Monitor** จากนั้น ภายใต้ การกําหนด **ค่า** ให้เลือก [รายงาน](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)การเข้ารหัสลับ</span><span class="sxs-lookup"><span data-stu-id="8bbbe-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="8bbbe-107">ถ้าคุณพบว่า Bitlocker ไม่สามารถเปิดใช้งานตามที่คาดไว้หรือโปรไฟล์ที่ใช้เพื่อเปิดใช้งาน Bitlocker อยู่ในสถานะข้อผิดพลาด โปรดตรวจสอบรายงานการเข้ารหัสลับเพื่อให้เข้าใจสาเหตุที่ลักษณะการเกิดขึ้นได้ดีขึ้น</span><span class="sxs-lookup"><span data-stu-id="8bbbe-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="8bbbe-108">เมื่อต้องการค้นหารายละเอียดเกี่ยวกับวิธีการแปลรายงานรวมถึงค่าสถานะการเข้ารหัสลับต่างๆ ให้ดู[ตรวจสอบการเข้ารหัสลับอุปกรณ์ด้วย Intunes](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)</span><span class="sxs-lookup"><span data-stu-id="8bbbe-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="8bbbe-109">คุณควรทราบว่าอุปกรณ์ที่ใหม่กว่าหลายเครื่องที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับ Bitlocker โดยอัตโนมัติ ซึ่งจะถูกทริกเกอร์โดยไม่มีแอปพลิเคชันนโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="8bbbe-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="8bbbe-110">ซึ่งอาจส่งผลกระทบต่อการใช้นโยบายถ้ามีการกําหนดค่าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="8bbbe-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="8bbbe-111">ดู FAQ ต่อไปนี้เพื่อดูรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="8bbbe-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="8bbbe-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies intun1](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="8bbbe-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="8bbbe-113">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="8bbbe-113">**FAQ**</span></span>

<span data-ttu-id="8bbbe-114">Q: Windows รุ่นใดที่สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันจุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="8bbbe-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="8bbbe-115">A: การตั้งค่าใน นโยบายการป้องกันจุดสิ้นสุดของ Intuned จะถูกปรับใช้โดยใช้[Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="8bbbe-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="8bbbe-116">Windows ไม่รองรับ Bitlocker CSP ทุกรุ่นหรือทุกรุ่น</span><span class="sxs-lookup"><span data-stu-id="8bbbe-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="8bbbe-117">Q: Bitlocker สามารถเปิดใช้งานบนอุปกรณ์โดยไม่ต้องมีการโต้ตอบของผู้ใช้ได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="8bbbe-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="8bbbe-118">A: ถ้าตรงตามเงื่อนไขที่จําเป็นแล้วคุณจึงสามารถเปิดใช้งาน Bitlocker "Silent Encryption" ผ่าน Intunes ได้</span><span class="sxs-lookup"><span data-stu-id="8bbbe-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="8bbbe-119">ดูรายละเอียดของความต้องการของอุปกรณ์และการตั้งค่านโยบายตัวอย่างเพื่อเปิดใช้งานการเข้ารหัสลับแบบไม่ระบุข้อมูลในเอกสารต่อไปนี้: [เปิดใช้งานการเข้ารหัสลับ Bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)โดยไม่เปิด</span><span class="sxs-lookup"><span data-stu-id="8bbbe-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="8bbbe-120">Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของ OS ในวิธีการเข้ารหัสลับและจุดแข็งการเข้ารหัส (XTS-AES-128) จะปรับใช้นโยบายที่มีการตั้งค่าอื่นทริกเกอร์การเข้ารหัสลับไดรฟ์ใหม่ด้วยการตั้งค่าใหม่โดยอัตโนมัติหรือไม่</span><span class="sxs-lookup"><span data-stu-id="8bbbe-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="8bbbe-121">A: ไม่ได้</span><span class="sxs-lookup"><span data-stu-id="8bbbe-121">A: No.</span></span> <span data-ttu-id="8bbbe-122">เมื่อต้องการใช้การตั้งค่าการเข้ารหัสใหม่ ไดรฟ์จะต้องถูกถอดรหัสลับก่อน</span><span class="sxs-lookup"><span data-stu-id="8bbbe-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="8bbbe-123">**หมายเหตุ:** For devices being enrolled with Autopilot, the automatic encryption that would would occur during OOBE is not triggered until Intuned policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span><span class="sxs-lookup"><span data-stu-id="8bbbe-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="8bbbe-124">Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลจากแอปพลิเคชันนโยบาย Intuned อุปกรณ์จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="8bbbe-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="8bbbe-125">A: การเอานโยบายที่เกี่ยวข้องกับการเข้ารหัสลับออกไม่ส่งผลให้มีการเข้ารหัสลับไดรฟ์ที่ถูกกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="8bbbe-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="8bbbe-126">Q: เหตุใดนโยบายการปฏิบัติตามนโยบาย Intun1 จึงแสดงให้เห็นว่าอุปกรณ์ของฉันไม่เปิดใช้งาน Bitlocker แม้ว่าจะเป็นเพราะอะไร</span><span class="sxs-lookup"><span data-stu-id="8bbbe-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="8bbbe-127">A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบาย Intun <2> ใช้ไคลเอ็นต์การทดสอบสถานภาพของอุปกรณ์ Windows (DHA)</span><span class="sxs-lookup"><span data-stu-id="8bbbe-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="8bbbe-128">ไคลเอ็นต์นี้วัดสถานะอุปกรณ์เมื่อเริ่มระบบเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="8bbbe-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="8bbbe-129">ดังนั้นถ้ายังไม่ได้เริ่มต้นระบบใหม่เนื่องจากการเข้ารหัสลับ Bitlocker เสร็จสมบูรณ์แล้ว บริการไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ว่าใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="8bbbe-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 