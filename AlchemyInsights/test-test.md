---
title: เงื่อนไขที่ขาดหายไปจากการจัดเก็บคำศัพท์ออนไลน์ของ SharePoint
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053532"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="fc56f-102">การเปิดใช้งานการเข้ารหัสลับด้วย Bitlocker ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="fc56f-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="fc56f-103">นโยบายการป้องกันปลายทาง Intune สามารถใช้เพื่อกำหนดการตั้งค่าการเข้ารหัสลับ Boitlocker สำหรับอุปกรณ์ Windows ตามที่อธิบายไว้ใน: Windows10 (และรุ่นที่ใหม่กว่า) เพื่อป้องกันอุปกรณ์โดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="fc56f-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="fc56f-104">คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย bitlocker โดยอัตโนมัติซึ่งจะถูกทริกเกอร์โดยไม่มีแอพลิเคชันของนโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="fc56f-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="fc56f-105">ซึ่งอาจส่งผลกระทบต่อการประยุกต์ใช้นโยบายถ้าการตั้งค่าเริ่มต้นไม่ได้ถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="fc56f-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="fc56f-106">ดูคำถามที่พบบ่อยสำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="fc56f-106">See FAQ for more detail.</span></span>


<span data-ttu-id="fc56f-107">คำ ถามที่พบบ่อย: Windows รุ่นใดที่สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันปลายทาง</span><span class="sxs-lookup"><span data-stu-id="fc56f-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="fc56f-108"> A: การตั้งค่าในนโยบายการป้องกันการปลายทาง Intune จะดำเนินการโดยใช้ Bitlocker CSP</span><span class="sxs-lookup"><span data-stu-id="fc56f-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="fc56f-109">ไม่ใช่ทุกรุ่นหรือรุ่นของ Windows ที่สนับสนุน Bitlocker CSP 
     </span><span class="sxs-lookup"><span data-stu-id="fc56f-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="fc56f-110">ในเวลานี้ Windows รุ่น: องค์กร; การศึกษา, มือถือ, องค์กรมือถือและมืออาชีพ (ตั้งแต่สร้าง๑๘๐๙เป็นต้นไป) ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="fc56f-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="fc56f-111">ถาม: หากอุปกรณ์ถูกเข้ารหัสด้วย Bitlocker อยู่แล้วโดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับวิธีการเข้ารหัสและความแรงของรหัส (XTS-AES-๑๒๘) จะใช้นโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ที่มีการตั้งค่าใหม่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="fc56f-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="fc56f-112">A: ไม่</span><span class="sxs-lookup"><span data-stu-id="fc56f-112">A: No.</span></span> <span data-ttu-id="fc56f-113">เพื่อที่จะใช้การตั้งค่าการเข้ารหัสใหม่ไดรฟ์ต้องถูกถอดรหัสลับก่อน</span><span class="sxs-lookup"><span data-stu-id="fc56f-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="fc56f-114">หมายเหตุสำหรับอุปกรณ์ที่กำลังลงทะเบียนกับออโตไพลอตการเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นในระหว่าง OOBE จะไม่ถูกทริกเกอร์จนกว่านโยบาย Intune จะถูกประเมินซึ่งช่วยให้การตั้งค่านโยบายตามที่จะใช้ในตำแหน่งของค่าเริ่มต้นของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="fc56f-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="fc56f-115">Q ถ้าอุปกรณ์ถูกเข้ารหัสเป็นผลมาจากการประยุกต์ใช้นโยบาย Intune จะถูกถอดรหัสลับเมื่อมีการเอานโยบายนั้นออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="fc56f-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="fc56f-116">A: การเอาออกของนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ส่งผลให้การถอดรหัสลับของไดรฟ์ที่ถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="fc56f-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="fc56f-117">ถาม: เหตุใดนโยบายการปฏิบัติตามกฎระเบียบ intune จึงแสดงว่าอุปกรณ์ของฉันไม่มี "เปิดใช้งาน Bitlocker" แต่เป็นอย่างไร</span><span class="sxs-lookup"><span data-stu-id="fc56f-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="fc56f-118">A: การตั้งค่า "Bitlocker เปิดใช้งาน" ในนโยบายการปฏิบัติตามกฎระเบียบ intune ใช้ไคลเอนต์การรับรองความสมบูรณ์ของอุปกรณ์ Windows (DHA)</span><span class="sxs-lookup"><span data-stu-id="fc56f-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="fc56f-119">ไคลเอนต์นี้วัดเฉพาะสถานะของอุปกรณ์ในเวลาบูต</span><span class="sxs-lookup"><span data-stu-id="fc56f-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="fc56f-120">ดังนั้นหากอุปกรณ์ไม่ได้ถูกรีบูตเนื่องจากการเข้ารหัสลับด้วย bitlocker เสร็จสมบูรณ์แล้วบริการไคลเอ็นต์ DHA จะไม่รายงาน bitlocker ขณะกำลังทำงานอยู่</span><span class="sxs-lookup"><span data-stu-id="fc56f-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>