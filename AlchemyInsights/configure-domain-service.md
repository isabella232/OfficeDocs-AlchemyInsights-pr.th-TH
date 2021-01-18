---
title: กำหนดค่าบริการโดเมน
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885685"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="618d9-102">ไม่สามารถเปิดใช้งาน AAD DS หรือการปรับใช้ที่ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="618d9-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="618d9-103">เมื่อต้องการแก้ไขปัญหาของบริการ Azure AD domain (AAD DS) ไม่ได้ถูกเปิดใช้งานหรือไม่สามารถปรับใช้ได้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="618d9-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="618d9-104">ถ้าคุณกำลังใช้เครือข่ายเสมือนที่มีอยู่แล้วให้ตรวจสอบ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ใน AAD DS https://aka.ms/aadds-networking ในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="618d9-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="618d9-105">ตรวจสอบเพื่อดูว่าข้อความแสดงข้อผิดพลาดของคุณได้รับคำตอบในคู่มือการแก้ไขปัญหานี้ที่พร้อมใช้งาน  https://aka.ms/aadds-troubleshoot-enable หรือไม่</span><span class="sxs-lookup"><span data-stu-id="618d9-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="618d9-106">ลองปรับใช้บริการ Domain AD Azure ในเครือข่ายเสมือนใหม่</span><span class="sxs-lookup"><span data-stu-id="618d9-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="618d9-107">ทำตามคู่มือการเริ่มต้นใช้งานในการปรับใช้ AAD DS:[สร้างและกำหนดค่าบริการ Domain Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="618d9-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="618d9-108">ถ้าคุณกำลังมีปัญหาเกี่ยวกับการปรับใช้บริการ Domain AD Azure ให้ดูที่การ [แก้ไขปัญหาของบริการ DOMAIN Ad azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) เพื่อแก้ไขข้อผิดพลาดทั่วไปเพื่อช่วยให้คุณทำสิ่งต่างๆได้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="618d9-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="618d9-109">**ไม่สามารถปิดใช้งาน AAD DS ได้**</span><span class="sxs-lookup"><span data-stu-id="618d9-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="618d9-110">AAD-DS ไม่สามารถหยุดชั่วคราวได้</span><span class="sxs-lookup"><span data-stu-id="618d9-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="618d9-111">ถ้าคุณต้องการหยุดการใช้โดเมนที่มีการจัดการของคุณจะต้องถูกลบออก</span><span class="sxs-lookup"><span data-stu-id="618d9-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="618d9-112">เมื่อต้องการลบโดเมนที่มีการจัดการของคุณให้ดู[ลบบริการโดเมน AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)</span><span class="sxs-lookup"><span data-stu-id="618d9-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



