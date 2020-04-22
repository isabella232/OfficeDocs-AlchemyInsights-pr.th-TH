---
title: คําที่ขาดหายไปจากที่เก็บคําของ SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766872"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="9ca85-102">การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="9ca85-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="9ca85-103">นโยบายการป้องกันปลายทาง Intune สามารถใช้ในการกําหนดค่าการตั้งค่าการเข้ารหัสลับ Boitlocker สําหรับอุปกรณ์ Windows ตามที่อธิบายไว้ใน : Windows10 (และรุ่นที่ใหม่กว่า)</span><span class="sxs-lookup"><span data-stu-id="9ca85-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="9ca85-104">คุณควรทราบว่า อุปกรณ์รุ่นใหม่ๆ ที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย BitLocker อัตโนมัติซึ่งถูกทริกเกอร์โดยไม่มีการใช้นโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="9ca85-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="9ca85-105">ซึ่งอาจส่งผลกระทบต่อโปรแกรมประยุกต์ของนโยบายถ้ามีการกําหนดค่าการตั้งค่าเริ่มต้นที่ไม่ใช่</span><span class="sxs-lookup"><span data-stu-id="9ca85-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="9ca85-106">ดูคําถามที่พบบ่อยสําหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="9ca85-106">See FAQ for more detail.</span></span>


<span data-ttu-id="9ca85-107">คําถามที่ถามบ่อย Q: การเข้ารหัสอุปกรณ์สนับสนุน Windows รุ่นใดที่ใช้นโยบายการป้องกันปลายทาง</span><span class="sxs-lookup"><span data-stu-id="9ca85-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="9ca85-108"> a:การตั้งค่าในนโยบายการป้องกันปลายทาง Intune จะนํามาใช้โดยใช้ CSP Bitlocker</span><span class="sxs-lookup"><span data-stu-id="9ca85-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="9ca85-109">รุ่นทั้งหมดหรือสร้างของ Windows ไม่สนับสนุน Bitlocker CSP 
     </span><span class="sxs-lookup"><span data-stu-id="9ca85-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="9ca85-110">ในเวลานี้ Windows รุ่น: องค์กร; สนับสนุนการศึกษา อุปกรณ์เคลื่อนที่ Mobile Enterprise และ Professional (จากรุ่น 1809 เป็นต้นไป)</span><span class="sxs-lookup"><span data-stu-id="9ca85-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="9ca85-111">ถาม: หากอุปกรณ์ถูกเข้ารหัสด้วย Bitlocker อยู่แล้วโดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสําหรับวิธีการเข้ารหัสและความแรงของการเข้ารหัส (XTS-AES-128) จะใช้นโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทําให้เกิดการเข้ารหัสของไดรฟ์ด้วยการตั้งค่าใหม่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="9ca85-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="9ca85-112">A: ไม่</span><span class="sxs-lookup"><span data-stu-id="9ca85-112">A: No.</span></span> <span data-ttu-id="9ca85-113">เพื่อที่จะใช้การตั้งค่าการเข้ารหัสใหม่ไดรฟ์จะต้องถูกถอดรหัสลับก่อน</span><span class="sxs-lookup"><span data-stu-id="9ca85-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="9ca85-114">หมายเหตุ สําหรับอุปกรณ์ที่กําลังลงทะเบียนกับ Autopilot การเข้ารหัสลับอัตโนมัติที่อาจเกิดขึ้นในระหว่าง OOBE จะไม่ถูกทริกเกอร์จนกว่านโยบาย Intune จะถูกประเมินซึ่งช่วยให้การตั้งค่าตามนโยบายที่จะใช้แทนค่าเริ่มต้นของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="9ca85-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="9ca85-115">Q หากอุปกรณ์ถูกเข้ารหัสเนื่องจากการประยุกต์ใช้นโยบาย Intune จะถูกถอดรหัสเมื่อนโยบายนั้นถูกเอาออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="9ca85-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="9ca85-116">A:การเอานโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ส่งผลในการถอดรหัสของไดรฟ์ที่ถูกกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="9ca85-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="9ca85-117">ถาม: เหตุใดนโยบายการปฏิบัติตามกฎระเบียบแสดงว่าอุปกรณ์ของฉันไม่มี "เปิดใช้งาน Bitlocker" แต่เป็นหรือไม่</span><span class="sxs-lookup"><span data-stu-id="9ca85-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="9ca85-118">การตั้งค่า "Bitlocker ที่เปิดใช้งาน" ในนโยบายการปฏิบัติตามนโยบาย intune ใช้ไคลเอ็นต์ของ Windows อุปกรณ์สุขภาพ Attestation (DHA)</span><span class="sxs-lookup"><span data-stu-id="9ca85-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="9ca85-119">ไคลเอ็นต์นี้วัดสถานะอุปกรณ์ในเวลาบูตเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="9ca85-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="9ca85-120">ดังนั้นหากอุปกรณ์ไม่ได้รับการเริ่มระบบใหม่เนื่องจากการเข้ารหัสลับด้วย BitLocker เสร็จสมบูรณ์บริการไคลเอ็นต์ DHA จะไม่รายงาน bitlocker เป็นที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="9ca85-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>