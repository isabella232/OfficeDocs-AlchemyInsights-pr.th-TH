---
title: ตัวควบคุมโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901316"
---
# <a name="domain-controller"></a><span data-ttu-id="437ed-102">ตัวควบคุมโดเมน</span><span class="sxs-lookup"><span data-stu-id="437ed-102">Domain controller</span></span>

<span data-ttu-id="437ed-103">**ไม่สามารถเปิดใช้งาน AAD DS หรือการปรับใช้ที่ล้มเหลว**</span><span class="sxs-lookup"><span data-stu-id="437ed-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="437ed-104">เมื่อต้องการแก้ไขปัญหาของบริการ Azure AD domain (AAD DS) ไม่ได้ถูกเปิดใช้งานหรือไม่สามารถปรับใช้ได้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="437ed-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="437ed-105">ถ้าคุณกำลังใช้เครือข่ายเสมือนที่มีอยู่แล้วให้ตรวจสอบ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ใน AAD DS https://aka.ms/aadds-networking ในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="437ed-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="437ed-106">ตรวจสอบเพื่อดูว่าข้อความแสดงข้อผิดพลาดของคุณได้รับคำตอบในคู่มือการแก้ไขปัญหานี้ที่พร้อมใช้งาน  https://aka.ms/aadds-troubleshoot-enable หรือไม่</span><span class="sxs-lookup"><span data-stu-id="437ed-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="437ed-107">ลองปรับใช้บริการ Domain AD Azure ในเครือข่ายเสมือนใหม่</span><span class="sxs-lookup"><span data-stu-id="437ed-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="437ed-108">ทำตามคู่มือเริ่มต้นใช้งานเกี่ยวกับวิธีการปรับใช้ AAD DS ซึ่งพร้อมใช้งานที่[บทช่วยสอนการสร้างบริการ DOMAIN AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="437ed-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="437ed-109">ถ้าคุณกำลังมีปัญหาเกี่ยวกับการปรับใช้บริการ Domain AD Azure ให้ดูที่การ [แก้ไขปัญหาของบริการ DOMAIN Ad azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) เพื่อแก้ไขข้อผิดพลาดทั่วไปเพื่อช่วยให้คุณทำสิ่งต่างๆได้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="437ed-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="437ed-110">**ไม่สามารถปิดใช้งาน AAD DS ได้**</span><span class="sxs-lookup"><span data-stu-id="437ed-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="437ed-111">AAD-DS ไม่สามารถหยุดชั่วคราวได้</span><span class="sxs-lookup"><span data-stu-id="437ed-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="437ed-112">ถ้าคุณต้องการหยุดการใช้โดเมนที่มีการจัดการของคุณจะต้องถูกลบออก</span><span class="sxs-lookup"><span data-stu-id="437ed-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="437ed-113">ถ้าคุณพบปัญหาในการแก้ไขข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ไขปัญหาที่เกี่ยวข้องเพื่อช่วยให้คุณทำสิ่งต่างๆให้เสร็จได้ให้ดูที่ [แก้ไขปัญหาบริการโดเมน](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)ของ active Directory ของ Azure</span><span class="sxs-lookup"><span data-stu-id="437ed-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
