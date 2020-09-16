---
title: เงื่อนไขที่หายไปจากที่เก็บคำของ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750470"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f7d70-102">การเปิดใช้งานการเข้ารหัสลับ Bitlocker ด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="f7d70-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="f7d70-103">นโยบายการป้องกันจุดสิ้นสุดของ Intune สามารถใช้ในการกำหนดค่าการตั้งค่าการเข้ารหัสลับ Boitlocker สำหรับอุปกรณ์ Windows ตามที่อธิบายไว้ใน: Windows10 (และใหม่กว่า) การตั้งค่าเพื่อป้องกันอุปกรณ์โดยใช้ Intune</span><span class="sxs-lookup"><span data-stu-id="f7d70-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="f7d70-104">คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย bitlocker โดยอัตโนมัติที่ทริกเกอร์โดยไม่มีแอปพลิเคชันของนโยบาย MDM</span><span class="sxs-lookup"><span data-stu-id="f7d70-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f7d70-105">การทำเช่นนี้อาจส่งผลกระทบต่อการใช้นโยบายถ้าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้นถูกกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="f7d70-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="f7d70-106">ดูคำถามที่ถามบ่อยสำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="f7d70-106">See FAQ for more detail.</span></span>


<span data-ttu-id="f7d70-107">คำถามที่ถามบ่อย   : คำถามที่ถามบ่อย: Windows สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันจุดสิ้นสุดหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f7d70-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="f7d70-108"> A: การตั้งค่าในนโยบายการป้องกันจุดสิ้นสุดของ Intune จะถูกนำไปใช้โดยใช้ CSP ของ Bitlocker</span><span class="sxs-lookup"><span data-stu-id="f7d70-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="f7d70-109">ไม่ใช่เวอร์ชันทั้งหมดหรือรุ่นของ Windows สนับสนุน Bitlocker CSP 
     </span><span class="sxs-lookup"><span data-stu-id="f7d70-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="f7d70-110">ในตอนนี้ Windows รุ่น: Enterprise; การศึกษา, โทรศัพท์มือถือ, องค์กรมือถือและมืออาชีพ (จากรุ่น๑๘๐๙เป็นต้นไป) ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="f7d70-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="f7d70-111">Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับการเข้ารหัสลับและความแรงของการเข้ารหัส (XTS-AES-๑๒๘) จะนำนโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ด้วยการตั้งค่าใหม่อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="f7d70-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="f7d70-112">A: ไม่ใช่</span><span class="sxs-lookup"><span data-stu-id="f7d70-112">A: No.</span></span> <span data-ttu-id="f7d70-113">เมื่อต้องการนำการตั้งค่าการเข้ารหัสใหม่ไปใช้ก่อนที่คุณจะต้องถอดรหัสลับไดรฟ์ออกก่อน</span><span class="sxs-lookup"><span data-stu-id="f7d70-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="f7d70-114">หมายเหตุสำหรับอุปกรณ์ที่ลงทะเบียนด้วย Autopilot การเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นระหว่าง OOBE จะไม่ทริกเกอร์จนกว่าจะมีการประเมินนโยบายของ Intune จนกว่าจะมีการประเมินนโยบายของ Intune ที่อนุญาตให้ใช้การตั้งค่านโยบายที่จะใช้แทนที่ค่าเริ่มต้นของระบบปฏิบัติการ</span><span class="sxs-lookup"><span data-stu-id="f7d70-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="f7d70-115">Q ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลลัพธ์ของแอปพลิเคชันของ Intune ของ Intune จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="f7d70-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="f7d70-116">A: การลบนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ทำให้เกิดการถอดรหัสลับของไดรฟ์ที่ได้รับการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="f7d70-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="f7d70-117">Q: เหตุใดนโยบายการปฏิบัติตามนโยบายของ intune ของ intune จึงแสดงว่าอุปกรณ์ของฉันไม่มี "Bitlocker เปิดใช้งาน" แต่จะเป็นอย่างไร</span><span class="sxs-lookup"><span data-stu-id="f7d70-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="f7d70-118">A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบายของ intune ใช้ไคลเอ็นต์ Windows อุปกรณ์สถานภาพรับรอง (DHA)</span><span class="sxs-lookup"><span data-stu-id="f7d70-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f7d70-119">ไคลเอ็นต์นี้จะวัดสถานะอุปกรณ์ในเวลาเริ่มต้นเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="f7d70-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="f7d70-120">ดังนั้นถ้าอุปกรณ์ยังไม่ได้รับการรีบูตเนื่องจากการเข้ารหัสลับด้วย bitlocker เสร็จสมบูรณ์บริการไคลเอ็นต์ของ DHA จะไม่รายงาน bitlocker เป็นการใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="f7d70-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>