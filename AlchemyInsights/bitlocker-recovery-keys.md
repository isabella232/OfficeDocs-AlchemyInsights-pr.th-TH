---
title: คีย์การกู้คืน Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505087"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="c1490-102">การเข้าถึงคีย์การกู้คืน Bitlocker</span><span class="sxs-lookup"><span data-stu-id="c1490-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="c1490-103">เมื่อกําหนดการตั้งค่า Bitlocker Intuned Endpoint Protection Policy คุณจะสามารถกําหนดได้ว่าควรจัดเก็บข้อมูลการกู้คืน Bitlocker ใน Azure Active Directory หรือไม่</span><span class="sxs-lookup"><span data-stu-id="c1490-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="c1490-104">ถ้ามีการกําหนดค่าการตั้งค่าดังกล่าว ผู้ดูแลระบบ Intun1 ควรมองเห็นข้อมูลการกู้คืนที่เก็บไว้โดยเป็นส่วนหนึ่งของข้อมูลระเบียนอุปกรณ์ในอุปกรณ์ Intuns blade ด้วยสองวิธี:</span><span class="sxs-lookup"><span data-stu-id="c1490-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="c1490-105">อุปกรณ์ - อุปกรณ์ Azure AD -> "อุปกรณ์" หรือ ->อุปกรณ์ทั้งหมด -> "อุปกรณ์" ->คีย์การกู้คืน</span><span class="sxs-lookup"><span data-stu-id="c1490-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="c1490-106">อีกวิธีหนึ่งคือ ถ้ามีการเข้าถึงแบบผู้ดูแลระบบไปยังอุปกรณ์ นั้น สามารถมองเห็นคีย์การกู้คืน (รหัสผ่าน) โดยการเรียกใช้การสั่งต่อไปนี้จากพร้อมท์สั่งผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="c1490-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="c1490-107">ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อนการลงทะเบียน intuned คีย์การกู้คืนอาจเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการลงชื่อเข้าใช้อุปกรณ์ในระหว่างกระบวนการ OOBE</span><span class="sxs-lookup"><span data-stu-id="c1490-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="c1490-108">ถ้าเป็นกรณีนี้ การเข้าถึง  https://onedrive.live.com/recoverykey และการลงชื่อเข้าใช้ด้วย MSA ควรแสดงอุปกรณ์ที่จัดเก็บคีย์การกู้คืนไว้</span><span class="sxs-lookup"><span data-stu-id="c1490-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="c1490-109">ถ้าอุปกรณ์ถูกเข้ารหัสลับเนื่องจากผลลัพธ์ของการกําหนดค่าผ่านนโยบายกลุ่มที่ยึดตามโดเมน ข้อมูลการกู้คืนอาจถูกจัดเก็บไว้ใน Active Directory ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="c1490-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="c1490-110">ถ้าคุณได้กําหนดค่านโยบายการป้องกันจุดสิ้นสุดเพื่อจัดเก็บคีย์การกู้คืนใน Azure Active Directory แต่ยังไม่ได้อัปโหลดคีย์บนอุปกรณ์ที่ระบุ คุณสามารถทริกเกอร์การอัปโหลดโดยการหมุนคีย์การกู้คืนของอุปกรณ์นั้นจากคอนโซล MEM</span><span class="sxs-lookup"><span data-stu-id="c1490-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="c1490-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="c1490-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

