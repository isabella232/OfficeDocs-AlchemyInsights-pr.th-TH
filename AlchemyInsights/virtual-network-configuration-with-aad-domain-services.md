---
title: การกำหนดค่าเสมือนกับบริการโดเมน AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885652"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="64809-102">การกำหนดค่าเสมือนกับบริการโดเมน AAD</span><span class="sxs-lookup"><span data-stu-id="64809-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="64809-103">การกำหนดค่าเสมือนกับบริการโดเมน AAD มีขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="64809-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="64809-104">การตรวจสอบสถานภาพโดเมนของคุณบนพอร์ทัล Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="64809-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="64809-105">การตรวจสอบการ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ในบริการโดเมน AD Azure บนพอร์ทัล https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="64809-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="64809-106">ตรวจสอบให้แน่ใจว่าเครือข่ายเสมือนของคุณได้รับการปรับใช้ในภูมิภาค Azure เดียวกันกับโดเมนที่มีการจัดการบริการ Domain AD Azure ของคุณ</span><span class="sxs-lookup"><span data-stu-id="64809-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="64809-107">ตรวจสอบให้แน่ใจว่าคุณไม่มีโดเมนที่มีอยู่ที่มีชื่อโดเมนเดียวกันกับที่มีอยู่บนเครือข่ายเสมือน</span><span class="sxs-lookup"><span data-stu-id="64809-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="64809-108">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการพิจารณาการออกแบบบนเครือข่ายเสมือนของ Azure เพื่อสนับสนุนบริการ domain domain ให้ดูที่การ[พิจารณาเครือข่ายเสมือน](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)</span><span class="sxs-lookup"><span data-stu-id="64809-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

