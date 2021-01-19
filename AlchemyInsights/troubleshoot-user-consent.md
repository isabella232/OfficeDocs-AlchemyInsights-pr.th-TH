---
title: การแก้ไขปัญหาความยินยอมของผู้ใช้
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901627"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="404bd-102">การแก้ไขปัญหาความยินยอมของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="404bd-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="404bd-103">คุณสามารถกำหนดค่าความยินยอมของผู้ใช้ไปยังแอปพลิเคชันผ่านทางพอร์ทัล Azure หรือ PowerShell ได้</span><span class="sxs-lookup"><span data-stu-id="404bd-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="404bd-104">สำหรับข้อมูลเพิ่มเติมให้ดูที่[การตั้งค่าความยินยอมของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)</span><span class="sxs-lookup"><span data-stu-id="404bd-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="404bd-105">ผู้ดูแลระบบยังสามารถใช้ API ของ [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) เพื่อให้ความยินยอมในการมอบสิทธิ์ในนามของผู้ใช้คนเดียวได้</span><span class="sxs-lookup"><span data-stu-id="404bd-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="404bd-106">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่รับสิทธิ์การเข้าถึงในนามของผู้ใช้](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="404bd-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="404bd-107">[ข้อผิดพลาดในการยินยอมของผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): บทความนี้จะอธิบายข้อผิดพลาดที่อาจเกิดขึ้นในระหว่างกระบวนการยินยอมให้กับแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="404bd-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="404bd-108">ถ้าคุณกำลังแก้ไขปัญหาพร้อมท์การยินยอมที่ไม่คาดคิดที่ไม่มีข้อความแสดงข้อผิดพลาดให้ดูที่[สถานการณ์การรับรองความถูกต้องสำหรับ AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="404bd-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>