---
title: การซิงโครไนซ์แฮชของรหัสผ่านกับบริการโดเมน
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177619"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="07f32-102">การซิงโครไนซ์แฮชของรหัสผ่านกับบริการโดเมน</span><span class="sxs-lookup"><span data-stu-id="07f32-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="07f32-103">**ถ้าอินสแตนซ์ Azure AD DS ของคุณพร้อมท์ให้คุณเปิดใช้งานการซิงโครไนซ์แฮชของรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="07f32-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="07f32-104">คุณพบกับสถานการณ์สมมติที่คุณเรียกใช้สภาพแวดล้อมแบบไฮบริดกับผู้ใช้ที่ซิงโครไนซ์จากสภาพแวดล้อม Azure Active Directory Domain Services (AD DS) ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="07f32-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="07f32-105">สถานการณ์นี้จะพบแม้คุณจะมีการซิงโครไนซ์แฮชรหัสผ่านจาก AD DS ภายในองค์กรไปยังผู้เช่า Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="07f32-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="07f32-106">**สาเหตุ**</span><span class="sxs-lookup"><span data-stu-id="07f32-106">**Cause**</span></span>

<span data-ttu-id="07f32-107">ปัญหานี้เกิดขึ้นเนื่องจาก Azure AD Connect ตามค่าเริ่มต้นจะไม่ซิงโครไนซ์ Hashes ของ Technology LAN แบบดั้งเดิม (NTLM) และ Kerberos Password Hashes ที่ต้องใช้ใน Azure AD DS</span><span class="sxs-lookup"><span data-stu-id="07f32-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="07f32-108">**วิธีแก้ไขปัญหาชั่วคราว**</span><span class="sxs-lookup"><span data-stu-id="07f32-108">**Workaround**</span></span> 

<span data-ttu-id="07f32-109">คุณจะต้องกําหนดค่า Azure AD Connect เพื่อซิงโครไนซ์ Hashes รหัสผ่านที่ต้องใช้ในการรับรองความถูกต้องของ NTLM และ Kerberos</span><span class="sxs-lookup"><span data-stu-id="07f32-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="07f32-110">หลังจากกําหนดค่า Azure AD Connect แล้ว การสร้างบัญชีภายในองค์กรหรือเหตุการณ์การเปลี่ยนรหัสผ่านจะซิงโครไนซ์ Hashe ของรหัสผ่านดั้งเดิมกับ Azure AD ด้วย</span><span class="sxs-lookup"><span data-stu-id="07f32-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="07f32-111">โปรดดู [ที่นี่](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งนี้และสําหรับแนวทางเกี่ยวกับวิธีการเปิดใช้งานการซิงโครไนซ์รหัสผ่านในสภาพแวดล้อมแบบไฮบริดของ Azure AD DS</span><span class="sxs-lookup"><span data-stu-id="07f32-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>