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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505013"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="fb6f3-102">การเข้าถึงแบบมีเงื่อนไขกับ Intune</span><span class="sxs-lookup"><span data-stu-id="fb6f3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="fb6f3-103">การใช้การ**เข้าถึง**แบบมีเงื่อนไขกับ Intune ต้องการขั้นตอน 3:</span><span class="sxs-lookup"><span data-stu-id="fb6f3-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="fb6f3-104">สร้าง**นโยบายการเข้าถึง**แบบมีเงื่อนไขที่กำหนดว่าทรัพยากรใดได้รับการป้องกันและจะต้องพบกับเงื่อนไขใดบ้างในการเข้าถึงทรัพยากรเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="fb6f3-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="fb6f3-105">ตัวอย่างเช่นอุปกรณ์ต้องสอดคล้องกันก่อนที่จะเข้าถึงเมลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="fb6f3-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="fb6f3-106">สร้าง**นโยบายการปฏิบัติตามกฎระเบียบ**เพื่อกำหนดการตั้งค่าที่ต้องได้รับก่อนที่อุปกรณ์จะถือว่าเป็นไปตามมาตรฐาน</span><span class="sxs-lookup"><span data-stu-id="fb6f3-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="fb6f3-107">ตัวอย่างเช่นอุปกรณ์ต้องมี pin อย่างน้อย6หลักก่อนที่จะถือว่าเป็นไปตามมาตรฐาน</span><span class="sxs-lookup"><span data-stu-id="fb6f3-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="fb6f3-108">การสร้างความมั่นใจใน**นโยบายการปฏิบัติตามกฎระเบียบ**และ**นโยบายการเข้าถึง**แบบมีเงื่อนไขจะถูกกำหนดเป้าหมายไปยังกลุ่มผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="fb6f3-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="fb6f3-109">ซึ่งอาจจำเป็นต้องสร้างกลุ่มผู้ใช้เฉพาะในไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="fb6f3-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="fb6f3-110">อ่านเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="fb6f3-110">Read more:</span></span>
  
- [<span data-ttu-id="fb6f3-111">แนวทางที่พึงปฏิบัติ</span><span class="sxs-lookup"><span data-stu-id="fb6f3-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="fb6f3-112">การเริ่มต้นใช้งานการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="fb6f3-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

