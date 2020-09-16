---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731258"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="dc0f5-102">การเปิดใช้งานการเข้ารหัสลับ Bitlocker ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="dc0f5-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="dc0f5-103">นโยบายการป้องกันจุดสิ้นสุดของ Intune สามารถใช้เพื่อกำหนดการตั้งค่าการเข้ารหัสลับของ Bitlocker สำหรับอุปกรณ์ Windows</span><span class="sxs-lookup"><span data-stu-id="dc0f5-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="dc0f5-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การตั้งค่า Windows 10 (และเวอร์ชันที่ใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="dc0f5-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="dc0f5-105">คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย Bitlocker โดยอัตโนมัติซึ่งจะถูกทริกเกอร์โดยไม่มีแอปพลิเคชันของนโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="dc0f5-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="dc0f5-106">การทำเช่นนี้อาจส่งผลกระทบต่อการใช้นโยบายถ้าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้นถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="dc0f5-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="dc0f5-107">ดูคำถามที่ถามบ่อยต่อไปนี้สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="dc0f5-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="dc0f5-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาของ bitlocker ให้ดู[ที่แก้ไขปัญหานโยบาย bitlocker ใน Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)</span><span class="sxs-lookup"><span data-stu-id="dc0f5-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="dc0f5-109">**คำถามที่ถามบ่อย**</span><span class="sxs-lookup"><span data-stu-id="dc0f5-109">**FAQ**</span></span>

 <span data-ttu-id="dc0f5-110">Q: รุ่นของการเข้ารหัสลับอุปกรณ์ของ Windows ที่สนับสนุนโดยใช้นโยบายการป้องกันจุดสิ้นสุดหรือไม่</span><span class="sxs-lookup"><span data-stu-id="dc0f5-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="dc0f5-111">A: การตั้งค่าในนโยบายการป้องกันจุดสิ้นสุดของ Intune จะถูกนำไปใช้โดยใช้[CSP ของ Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="dc0f5-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="dc0f5-112">ไม่ใช่เวอร์ชันหรือรุ่นทั้งหมดของ Windows สนับสนุน Bitlocker CSP</span><span class="sxs-lookup"><span data-stu-id="dc0f5-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="dc0f5-113">ในตอนนี้ Windows รุ่นต่อไปนี้ได้รับการสนับสนุน: Enterprise, Education, Mobile, mobile Enterprise และ Professional (รุ่น๑๘๐๙และเวอร์ชันที่ใหม่กว่า)</span><span class="sxs-lookup"><span data-stu-id="dc0f5-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="dc0f5-114">Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับการเข้ารหัสลับและความแรงของการเข้ารหัส (XTS-AES-๑๒๘) จะนำนโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ด้วยการตั้งค่าใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="dc0f5-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="dc0f5-115">A: ไม่ใช่</span><span class="sxs-lookup"><span data-stu-id="dc0f5-115">A: No.</span></span> <span data-ttu-id="dc0f5-116">เมื่อต้องการนำการตั้งค่าการเข้ารหัสใหม่ไปใช้ไดรฟ์จะต้องถอดรหัสลับก่อน</span><span class="sxs-lookup"><span data-stu-id="dc0f5-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="dc0f5-117">**หมายเหตุ:** สำหรับอุปกรณ์ที่กำลังลงทะเบียนกับ Autopilot การเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นระหว่าง OOBE จะไม่ทริกเกอร์จนกว่าจะมีการประเมินนโยบาย Intune จนกว่าจะมีการประเมินนโยบายของ Intune ซึ่งจะทำให้การตั้งค่านโยบายถูกนำไปใช้แทนที่ค่าเริ่มต้นของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="dc0f5-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="dc0f5-118">Q: ถ้าอุปกรณ์ได้รับการเข้ารหัสลับเป็นผลลัพธ์ของแอปพลิเคชัน Intune ของ Intune จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="dc0f5-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="dc0f5-119">A: การลบนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ทำให้เกิดการถอดรหัสลับของไดรฟ์ที่ได้รับการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="dc0f5-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="dc0f5-120">Q: เหตุใดนโยบายการปฏิบัติตามนโยบายของ Intune ของ Intune จึงแสดงว่าอุปกรณ์ของฉันไม่ได้เปิดใช้งาน Bitlocker แม้ว่าจะเป็นใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="dc0f5-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="dc0f5-121">A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบายของ Intune ที่ใช้ไคลเอ็นต์ Windows อุปกรณ์สถานภาพรับรอง (DHA)</span><span class="sxs-lookup"><span data-stu-id="dc0f5-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="dc0f5-122">ไคลเอ็นต์นี้จะวัดสถานะอุปกรณ์ในเวลาเริ่มต้นเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="dc0f5-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="dc0f5-123">ดังนั้นถ้าอุปกรณ์ยังไม่ได้รับการรีบูตเนื่องจากการเข้ารหัสลับด้วย Bitlocker เสร็จสมบูรณ์บริการของไคลเอ็นต์ DHA จะไม่รายงาน Bitlocker ที่กำลังถูกใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="dc0f5-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 