---
title: ปัญหาการเตรียมใช้งาน SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949950"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="43cf5-102">ปัญหาการเตรียมใช้งาน SCIM</span><span class="sxs-lookup"><span data-stu-id="43cf5-102">SCIM provisioning issue</span></span>

<span data-ttu-id="43cf5-103">การจัดเตรียมอัตโนมัติอ้างอิงถึงการสร้างข้อมูลเฉพาะตัวของผู้ใช้และบทบาทในแอปพลิเคชัน cloud ที่ผู้ใช้ต้องการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="43cf5-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="43cf5-104">นอกเหนือจากการสร้างข้อมูลเฉพาะตัวของผู้ใช้การเตรียมใช้งานอัตโนมัติจะรวมถึงการบำรุงรักษาและการเอาข้อมูลประจำตัวของผู้ใช้ออกเป็นสถานะหรือบทบาทการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="43cf5-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="43cf5-105">ก่อนที่คุณจะเริ่มต้นการปรับใช้คุณสามารถตรวจสอบ [วิธีการเตรียมใช้งานการทำงาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) เพื่อเรียนรู้วิธีการเตรียมใช้งานการเตรียมใช้งานของ Azure active DIRECTORY (AD) และรับคำแนะนำในการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="43cf5-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="43cf5-106">ในฐานะนักพัฒนาแอปพลิเคชันคุณสามารถใช้ API สำหรับการจัดการผู้ใช้ข้อมูลประจำตัวแบบข้ามโดเมน (SCIM) เพื่อเปิดใช้งานการเตรียมใช้งานอัตโนมัติของผู้ใช้และกลุ่มระหว่างแอปพลิเคชันของคุณและ Azure AD</span><span class="sxs-lookup"><span data-stu-id="43cf5-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="43cf5-107">การ [สร้างจุดสิ้นสุด SCIM และกำหนดค่าการเตรียมใช้งานของผู้ใช้ด้วยบทความ AD Azure](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) จะอธิบายวิธีการสร้างจุดสิ้นสุด SCIM และรวมเข้ากับบริการการเตรียมใช้งาน Azure AD</span><span class="sxs-lookup"><span data-stu-id="43cf5-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



