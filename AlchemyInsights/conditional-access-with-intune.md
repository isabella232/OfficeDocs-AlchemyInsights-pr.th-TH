---
title: การเข้าถึงแบบมีเงื่อนไขด้วย Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706040"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="177e7-102">การเข้าถึงแบบมีเงื่อนไขด้วย Intune</span><span class="sxs-lookup"><span data-stu-id="177e7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="177e7-103">การใช้**การเข้าถึงแบบมีเงื่อนไข**กับ Intune ต้องใช้ 3 ขั้นตอน:</span><span class="sxs-lookup"><span data-stu-id="177e7-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="177e7-104">สร้าง**นโยบายการเข้าถึงแบบมีเงื่อนไข**ที่กําหนดทรัพยากรใดที่จะถูกป้องกัน และเงื่อนไขที่จําเป็นต้องได้รับเพื่อเข้าถึงทรัพยากรเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="177e7-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="177e7-105">ตัวอย่างเช่น อุปกรณ์ต้องเป็นไปตามข้อกําหนดก่อนเข้าถึงอีเมลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="177e7-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="177e7-106">สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกําหนดการตั้งค่าที่ต้องเป็นไปตามก่อนที่อุปกรณ์จะถือว่าสอดคล้อง</span><span class="sxs-lookup"><span data-stu-id="177e7-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="177e7-107">ตัวอย่างเช่น อุปกรณ์ต้องมีหมุดอย่างน้อย 6 หลักก่อนที่จะถือว่าเป็นไปตามข้อกําหนด</span><span class="sxs-lookup"><span data-stu-id="177e7-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="177e7-108">การทําให้แน่ใจว่า**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึงแบบมีเงื่อนไข**จะกําหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="177e7-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="177e7-109">ซึ่งอาจต้องการสร้างกลุ่มเฉพาะของผู้ใช้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="177e7-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="177e7-110">อ่านเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="177e7-110">Read more:</span></span>
  
- [<span data-ttu-id="177e7-111">แนวทางปฏิบัติที่ดีที่สุดของการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="177e7-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="177e7-112">การเริ่มต้นใช้งานการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="177e7-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

