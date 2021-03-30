---
title: ปัญหาข้อมูลลับหรือใบรับรองของไคลเอ็นต์การลงทะเบียนแอป
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405330"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="93bdd-102">ปัญหาความลับหรือใบรับรองของไคลเอ็นต์การลงทะเบียนแอป</span><span class="sxs-lookup"><span data-stu-id="93bdd-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="93bdd-103">ไคลเอ็นต์แอปพลิเคชันหมดอายุลงหรือไม่</span><span class="sxs-lookup"><span data-stu-id="93bdd-103">Application client secret expiring?</span></span>

<span data-ttu-id="93bdd-104">ไม่ว่าจะสร้างแอปพลิเคชันที่ลงทะเบียนไว้อย่างไร ไม่ว่าจะผ่านขั้นตอนการลงทะเบียนมาตรฐานในพอร์ทัลการลงทะเบียนแอป หรือถ้าหลักของบริการถูกสร้างขึ้นในผู้เช่าของคุณโดยใช้ความยินยอมของแอปพลิเคชัน ข้อมูลลับไคลเอ็นต์ใหม่จะถูกสร้างขึ้นก่อนที่จะหมดอายุของรหัสแอปพลิเคชันปัจจุบันและถูกอัปเดตในรหัสแอปพลิเคชันที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="93bdd-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="93bdd-105">ระยะเวลาที่ใช้ได้สูงสุดคือ 2 ปี</span><span class="sxs-lookup"><span data-stu-id="93bdd-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="93bdd-106">ในฐานะที่เป็นตัวเตือน ค่าลับต้องถูกบันทึกเนื่องจากจะไม่สามารถมองเห็นได้อีกต่อไปหลังจากออกจากหน้าการลงทะเบียนแอปในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="93bdd-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="93bdd-107">ดูข้อมูลเริ่มต้นใช้งานด่วน:[ลงทะเบียนแอปในแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)และหลักปฏิบัติ[ที่ดีที่สุดเกี่ยวกับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="93bdd-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="93bdd-108">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [สร้างแอป Azure AD &หลักของบริการในพอร์ทัล - แพลตฟอร์มข้อมูลเฉพาะตัวของ](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)Microsoft</span><span class="sxs-lookup"><span data-stu-id="93bdd-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
