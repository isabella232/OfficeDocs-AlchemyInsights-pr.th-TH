---
title: คีย์การกู้คืนของ Bitlocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685905"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="694d7-102">การเข้าถึงคีย์การกู้คืนของ Bitlocker</span><span class="sxs-lookup"><span data-stu-id="694d7-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="694d7-103">เมื่อกำหนดค่านโยบายการป้องกันจุดสิ้นสุดของการตั้งค่า Bitlocker การป้องกันจุดสิ้นสุดคุณสามารถกำหนดได้ว่าควรเก็บข้อมูลการกู้คืนของ Bitlocker ไว้ใน Azure Active Directory หรือไม่</span><span class="sxs-lookup"><span data-stu-id="694d7-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="694d7-104">ถ้าการตั้งค่าดังกล่าวถูกกำหนดค่าข้อมูลการกู้คืนที่เก็บไว้ควรจะสามารถมองเห็นได้ในฐานะผู้ดูแลระบบ Intune ที่เป็นส่วนหนึ่งของข้อมูลระเบียนอุปกรณ์ในอุปกรณ์ Intune ที่ใช้งานได้สองวิธีดังนี้</span><span class="sxs-lookup"><span data-stu-id="694d7-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="694d7-105">อุปกรณ์-อุปกรณ์ Azure AD-> "อุปกรณ์" หรืออุปกรณ์-> อุปกรณ์ทั้งหมด-> "อุปกรณ์"-คีย์การกู้คืน ></span><span class="sxs-lookup"><span data-stu-id="694d7-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="694d7-106">อีกวิธีหนึ่งคือถ้ามีสิทธิ์ในการเข้าถึงอุปกรณ์ตัวเองคีย์การกู้คืน (รหัสผ่าน) สามารถเห็นได้โดยการเรียกใช้คำสั่งต่อไปนี้จากพร้อมท์คำสั่ง:</span><span class="sxs-lookup"><span data-stu-id="694d7-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="694d7-107">ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อนที่จะลงทะเบียนใน Intune คีย์การกู้คืนอาจถูกเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการลงชื่อเข้าใช้อุปกรณ์ในระหว่างกระบวนการ OOBE</span><span class="sxs-lookup"><span data-stu-id="694d7-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="694d7-108">ถ้าเป็นกรณีนี้การเข้าถึง  https://onedrive.live.com/recoverykey และการลงชื่อเข้าใช้ด้วย MSA ควรแสดงอุปกรณ์ที่มีการจัดเก็บคีย์การกู้คืน</span><span class="sxs-lookup"><span data-stu-id="694d7-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="694d7-109">ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลลัพธ์ของการกำหนดค่าผ่านทางนโยบายกลุ่มที่ใช้โดเมนข้อมูลการกู้คืนอาจถูกเก็บไว้ในไดเรกทอรีที่ใช้งานอยู่ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="694d7-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

