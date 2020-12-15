---
title: ตั้งค่าไดเรกทอรีที่ใช้งานอยู่ของ Azure
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004192"
- "7373"
ms.openlocfilehash: 94078246562112709eee303fa13d4ac2aa651b12
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679643"
---
# <a name="set-up-azure-active-directory"></a><span data-ttu-id="f205b-102">ตั้งค่าไดเรกทอรีที่ใช้งานอยู่ของ Azure</span><span class="sxs-lookup"><span data-stu-id="f205b-102">Set up Azure Active Directory</span></span>

<span data-ttu-id="f205b-103">[คู่มือการตั้งค่า AZURE AD](https://go.microsoft.com/fwlink/?linkid=2134390)ให้ข้อมูลเพื่อให้แน่ใจว่าองค์กรของคุณมีรากฐานความปลอดภัยที่เข้มงวด</span><span class="sxs-lookup"><span data-stu-id="f205b-103">The [Azure AD setup guide](https://go.microsoft.com/fwlink/?linkid=2134390) provides information to ensure your organization has a strong security foundation.</span></span> <span data-ttu-id="f205b-104">ในคู่มือนี้คุณจะตั้งค่าฟีเจอร์เริ่มต้นเช่นการควบคุมการเข้าถึงตามบทบาท Azure (Azure RBAC) สำหรับผู้ดูแลระบบ, Azure AD Connect สำหรับไดเรกทอรีภายในองค์กรของคุณและสถานภาพ Azure AD Connect เพื่อให้คุณสามารถตรวจสอบสถานภาพของข้อมูลประจำตัวแบบไฮบริดของคุณในระหว่างการซิงค์อัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f205b-104">In this guide you will set up initial features, like Azure role-based access control (Azure RBAC) for admins, Azure AD Connect for your on-premises directory, and Azure AD Connect Health, so you can monitor your hybrid identity's health during automated syncs.</span></span>

<span data-ttu-id="f205b-105">นอกจากนี้ยังมีข้อมูลที่จำเป็นในการเปิดใช้งานการตั้งค่ารหัสผ่านแบบบริการตนเองการเข้าถึงตามเงื่อนไขและการลงชื่อเข้าใช้แบบรวมของบริษัทอื่นรวมถึงการป้องกันข้อมูลประจำตัวขั้นสูงและการเตรียมการใช้งานอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="f205b-105">It also includes essential information on enabling self-service password resets, conditional access and integrated third-party sign-on including optional advanced identity protection and user provisioning automation.</span></span>
