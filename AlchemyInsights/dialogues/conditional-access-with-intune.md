---
title: การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694716"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="06d97-102">การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1</span><span class="sxs-lookup"><span data-stu-id="06d97-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="06d97-103">การใช้การเข้าถึงตามเงื่อนไขด้วย Intun1 ต้องมี 3 ขั้นตอน:</span><span class="sxs-lookup"><span data-stu-id="06d97-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="06d97-104">สร้างนโยบายการปฏิบัติตามนโยบายเพื่อกําหนดการตั้งค่าที่ต้องปฏิบัติตามก่อนที่จะถือว่าอุปกรณ์ปฏิบัติตามนโยบายแล้ว ตัวอย่างเช่น อุปกรณ์ต้องมีรหัส PIN อย่างน้อย 6 หลักก่อนที่จะถือว่าตรงตามมาตรฐาน</span><span class="sxs-lookup"><span data-stu-id="06d97-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="06d97-105">สร้างนโยบายการเข้าถึงตามเงื่อนไขที่กําหนดว่าทรัพยากรใดที่ได้รับการป้องกัน และเงื่อนไขที่ต้องใช้เพื่อเข้าถึงทรัพยากรเหล่านั้น ตัวอย่างเช่น อุปกรณ์จะต้องปฏิบัติตามนโยบายก่อนที่จะเข้าถึงอีเมลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="06d97-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="06d97-106">ตรวจสอบให้แน่ใจว่านโยบายการปฏิบัติตามนโยบายและนโยบายการเข้าถึงตามเงื่อนไขถูกตั้งเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ ซึ่งอาจต้องมีการสร้างกลุ่มเฉพาะของผู้ใช้ใน Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="06d97-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="06d97-107">อ่านเพิ่มเติม...</span><span class="sxs-lookup"><span data-stu-id="06d97-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
