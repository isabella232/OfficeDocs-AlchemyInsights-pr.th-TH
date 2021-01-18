---
title: ปัญหาในการเข้าร่วม VMs
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885659"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="0a561-102">ปัญหาในการเข้าร่วม VMs</span><span class="sxs-lookup"><span data-stu-id="0a561-102">Issue joining VMs</span></span>

<span data-ttu-id="0a561-103">เมื่อต้องการแก้ไขปัญหาที่เกิดขึ้นขณะพยายามเข้าร่วม VMs ให้ดำเนินการตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0a561-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="0a561-104">ลองลงชื่อเข้าใช้โดยใช้รูปแบบ **UPN** (ตัวอย่างเช่น ' joeuser@contoso.com ') แทนที่จะเป็นรูปแบบ **SAMAccountName** (' CONTOSO\joeuser ')</span><span class="sxs-lookup"><span data-stu-id="0a561-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="0a561-105">ตรวจสอบให้แน่ใจว่าคุณได้เปิดใช้งานการซิงโครไนซ์รหัสผ่านให้สอดคล้องกับขั้นตอนที่ระบุไว้ในคู่มือ *การเริ่มต้น* ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="0a561-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="0a561-106">ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ได้รับผลกระทบไม่ใช่บัญชีภายนอกในผู้เช่า Azure AD</span><span class="sxs-lookup"><span data-stu-id="0a561-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="0a561-107">ผู้ใช้ภายนอกไม่สามารถลงชื่อเข้าใช้โดเมนที่มีการจัดการได้เนื่องจากบริการ Domain AD Azure ไม่มีข้อมูลประจำตัวสำหรับบัญชีผู้ใช้ดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="0a561-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="0a561-108">ถ้าบัญชีผู้ใช้ที่ได้รับผลกระทบเป็นบัญชีผู้ใช้ cloud เท่านั้นให้ตรวจสอบให้แน่ใจว่าผู้ใช้ได้เปลี่ยนรหัสผ่านของพวกเขาหลังจากที่คุณเปิดใช้งาน Azure AD Domain Services แล้ว</span><span class="sxs-lookup"><span data-stu-id="0a561-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="0a561-109">ขั้นตอนนี้ทำให้เกิด hashes ข้อมูลประจำตัวที่จำเป็นสำหรับบริการโดเมน AD Azure ที่จะถูกสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="0a561-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="0a561-110">ถ้ามีการซิงโครไนซ์บัญชีผู้ใช้ที่ได้รับผลกระทบจากไดเรกทอรีภายในองค์กรให้ตรวจสอบว่ามีการกำหนดค่าการเผยแพร่ AD Azure ที่แนะนำให้ทำการซิงโครไนซ์ทั้งหมดหรือไม่</span><span class="sxs-lookup"><span data-stu-id="0a561-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="0a561-111">ถ้าปัญหายังคงมีอยู่หลังจากยืนยันขั้นตอนที่4ให้ดำเนินการคำสั่งต่อไปนี้จากเครื่องซิงค์ของคุณ:</span><span class="sxs-lookup"><span data-stu-id="0a561-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="0a561-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="0a561-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>