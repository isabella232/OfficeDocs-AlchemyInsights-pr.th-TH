---
title: ปัญหาเกี่ยวกับกลุ่มความปลอดภัย
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177635"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="98c15-102">ปัญหาเกี่ยวกับกลุ่มความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="98c15-102">Issue with security groups</span></span>

<span data-ttu-id="98c15-103">**ถ้าคุณได้รับข้อผิดพลาดเครือข่าย AADDS104**</span><span class="sxs-lookup"><span data-stu-id="98c15-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="98c15-104">กฎของกลุ่มความปลอดภัยของเครือข่ายไม่ถูกต้องเป็นสาเหตุที่พบบ่อยที่สุดของข้อผิดพลาดเครือข่ายของ Azure Active Directory Domain Services (AD DS)</span><span class="sxs-lookup"><span data-stu-id="98c15-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="98c15-105">กลุ่มความปลอดภัยของเครือข่ายของเครือข่ายเสมือนต้องอนุญาตให้เข้าถึงพอร์ตและโพรโทคอลเฉพาะได้</span><span class="sxs-lookup"><span data-stu-id="98c15-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="98c15-106">ถ้าพอร์ตเหล่านี้ถูกบล็อก แพลตฟอร์ม Azure ไม่สามารถตรวจสอบหรืออัปเดตโดเมนที่มีการจัดการได้</span><span class="sxs-lookup"><span data-stu-id="98c15-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="98c15-107">การซิงโครไนซ์ระหว่าง Azure AD และ Azure AD DS ยังได้รับผลกระทบอีกด้วย</span><span class="sxs-lookup"><span data-stu-id="98c15-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="98c15-108">ตรวจสอบให้แน่ใจว่าคุณเปิดพอร์ตเริ่มต้นไว้เพื่อไม่ให้บริการขัดข้อง</span><span class="sxs-lookup"><span data-stu-id="98c15-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="98c15-109">เมื่อต้องการเข้าใจและแก้ไขปัญหาการกําหนดค่ากลุ่มความปลอดภัยของเครือข่ายที่พบทั่วไป ให้ดูที่ [เพิ่มและตรวจสอบกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)ความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="98c15-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
