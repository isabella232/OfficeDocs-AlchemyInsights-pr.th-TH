---
title: การเข้าถึงแบบมีเงื่อนไขกับ Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935975"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="04931-102">การเข้าถึงแบบมีเงื่อนไขกับ Intune</span><span class="sxs-lookup"><span data-stu-id="04931-102">Conditional Access with Intune</span></span>

<span data-ttu-id="04931-103">ใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intune ต้องมีขั้นตอนที่ 3:</span><span class="sxs-lookup"><span data-stu-id="04931-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="04931-p101">สร้าง**นโยบายการเข้าถึงตามเงื่อนไข**ที่กำหนดทรัพยากรจะมีการป้องกัน และเงื่อนไขต้องมีสิ่งใดจะสามารถตอบสนองการเข้าถึงทรัพยากรดังกล่าว ตัวอย่างเช่น อุปกรณ์ต้องเข้ากันได้ก่อนที่จะเข้าถึงอีเมลขององค์กร</span><span class="sxs-lookup"><span data-stu-id="04931-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="04931-p102">สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกำหนดการตั้งค่าที่เป็นเงื่อนไขก่อนที่อุปกรณ์จะถือว่าเป็นไปตามกฎ ตัวอย่างเช่น อุปกรณ์ต้องมี pin ของตัวเลขอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามกฎ</span><span class="sxs-lookup"><span data-stu-id="04931-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="04931-p103">แน่ใจว่า ทั้ง**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงแบบมีเงื่อนไข**จะมุ่งเป้าไปยังกลุ่มที่ต้องการของผู้ใช้ ซึ่งอาจจำเป็นต้องสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="04931-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="04931-110">อ่านเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="04931-110">Read more:</span></span>
  
- [<span data-ttu-id="04931-111">วิธีปฏิบัติที่ดีที่สุดเข้าแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="04931-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="04931-112">เริ่มต้น ด้วยการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="04931-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

