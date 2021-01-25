---
title: สิทธิ์และความยินยอมของ API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974996"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="a8dba-102">สิทธิ์และความยินยอมของ API</span><span class="sxs-lookup"><span data-stu-id="a8dba-102">API permissions and consent</span></span>

<span data-ttu-id="a8dba-103">แอปพลิเคชันที่รวมเข้ากับ Microsoft identity platform จะทำตามรูปแบบการตรวจสอบที่ทำให้ผู้ใช้และผู้ดูแลระบบสามารถควบคุมได้ว่าจะสามารถเข้าถึงข้อมูลได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="a8dba-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="a8dba-104">การใช้งานของแบบจำลองการตรวจสอบได้รับการอัปเดตในจุดสิ้นสุดของแพลตฟอร์มสำหรับข้อมูลประจำตัวของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8dba-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="a8dba-105">การเปลี่ยนแปลงวิธีที่แอปจะต้องโต้ตอบกับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8dba-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="a8dba-106">[สิทธิ์และความยินยอมในจุดสิ้นสุดของแพลตฟอร์มสำหรับข้อมูลประจำ](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ตัวของ Microsoft ครอบคลุมแนวคิดพื้นฐานของรูปแบบการตรวจสอบนี้รวมถึงขอบเขตสิทธิ์และความยินยอม</span><span class="sxs-lookup"><span data-stu-id="a8dba-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="a8dba-107">[กรอบความยินยอมของ Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)ทำให้ง่ายต่อการพัฒนาเว็บไซต์ผู้เช่าหลายรายและแอปพลิเคชันไคลเอ็นต์ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="a8dba-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="a8dba-108">แอปพลิเคชันเหล่านี้อนุญาตให้เข้าสู่ระบบโดยบัญชีผู้ใช้จากผู้เช่าโฆษณา Azure ที่แตกต่างจากที่มีการลงทะเบียนแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="a8dba-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="a8dba-109">นอกจากนี้พวกเขาอาจจำเป็นต้องเข้าถึงเว็บ APIs เช่น Microsoft Graph API (ในการเข้าถึง Azure AD, Intune และบริการใน Microsoft ๓๖๕) และอื่นๆของ Microsoft services APIs นอกเหนือจากเว็บ APIs ของคุณเอง</span><span class="sxs-lookup"><span data-stu-id="a8dba-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

