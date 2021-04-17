---
title: คีย์การกู้คืน Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820305"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="83084-102">การเข้าถึงคีย์การกู้คืน Bitlocker</span><span class="sxs-lookup"><span data-stu-id="83084-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="83084-103">เมื่อกําหนดการตั้งค่า Bitlocker นโยบายการป้องกันปลายทาง Intuned คุณจะสามารถกําหนดได้ว่าข้อมูลการกู้คืน Bitlocker ควรจัดเก็บไว้ใน Azure Active Directory หรือไม่</span><span class="sxs-lookup"><span data-stu-id="83084-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="83084-104">ถ้าการตั้งค่าดังกล่าวได้รับการกําหนดค่า ผู้ดูแลระบบ Intun1 ควรเห็นข้อมูลการกู้คืนที่เก็บไว้โดยเป็นส่วนหนึ่งของข้อมูลระเบียนอุปกรณ์ในอุปกรณ์ Intuns blade ด้วยสองวิธี:</span><span class="sxs-lookup"><span data-stu-id="83084-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="83084-105">อุปกรณ์ - อุปกรณ์ Azure AD -> "อุปกรณ์" หรืออุปกรณ์ ->อุปกรณ์ทั้งหมด -> "อุปกรณ์" ->คีย์การกู้คืน</span><span class="sxs-lookup"><span data-stu-id="83084-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="83084-106">อีกวิธีหนึ่งคือ ถ้ามีการเข้าถึงแบบผู้ดูแลระบบไปยังอุปกรณ์ นั้น สามารถดูคีย์การกู้คืน (รหัสผ่าน) ได้โดยการเรียกใช้การสั่งต่อไปนี้จากพร้อมท์สั่งที่ยกระดับ:</span><span class="sxs-lookup"><span data-stu-id="83084-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="83084-107">ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อน enrolment intuned คีย์การกู้คืนอาจเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการลงชื่อเข้าใช้อุปกรณ์ในระหว่างกระบวนการ OOBE</span><span class="sxs-lookup"><span data-stu-id="83084-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="83084-108">ถ้าเป็นกรณีนี้ การเข้าถึงและการ  https://onedrive.live.com/recoverykey ลงชื่อเข้าใช้ด้วย MSA ควรแสดงอุปกรณ์ที่จัดเก็บคีย์การกู้คืนไว้</span><span class="sxs-lookup"><span data-stu-id="83084-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="83084-109">ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลลัพธ์ของการกําหนดค่าผ่านนโยบายกลุ่มที่ใช้โดเมน ข้อมูลการกู้คืนอาจถูกเก็บไว้ใน Active Directory ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="83084-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="83084-110">ถ้าคุณได้กําหนดค่านโยบายการป้องกันจุดสิ้นสุดเพื่อจัดเก็บคีย์การกู้คืนใน Azure Active Directory แต่ยังไม่ได้อัปโหลดคีย์ของอุปกรณ์ที่ระบุ คุณสามารถทริกเกอร์การอัปโหลดโดยการหมุนคีย์การกู้คืนของอุปกรณ์นั้นจากคอนโซล MEM</span><span class="sxs-lookup"><span data-stu-id="83084-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="83084-111">โปรดดูรายละเอียดที่[หมุนคีย์การกู้คืน BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="83084-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

