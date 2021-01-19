---
title: แก้ไขปัญหาของเจ้าของ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901275"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="54043-102">แก้ไขปัญหาของเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="54043-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="54043-103">เมื่อต้องการแก้ไขปัญหาที่เกี่ยวข้องกับเจ้าของให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="54043-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="54043-104">[เพิ่มหรือเปลี่ยนผู้ดูแลการสมัคร](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)ใช้งาน azure: กลุ่ม Azure active Directory (azure AD) จะเป็นเจ้าของและจัดการโดยเจ้าของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="54043-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="54043-105">เจ้าของกลุ่มสามารถเป็นผู้ใช้หรือการรักษาบริการและสามารถจัดการกลุ่มรวมถึงการเป็นสมาชิกได้</span><span class="sxs-lookup"><span data-stu-id="54043-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="54043-106">เฉพาะเจ้าของกลุ่มที่มีอยู่หรือผู้ดูแลระบบการจัดการกลุ่มเท่านั้นที่สามารถกำหนดเจ้าของกลุ่มได้</span><span class="sxs-lookup"><span data-stu-id="54043-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="54043-107">เจ้าของกลุ่มไม่จำเป็นต้องเป็นสมาชิกของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="54043-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="54043-108">[เพิ่มหรือเปลี่ยนผู้ดูแลการสมัคร](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)ใช้งาน Azure: บทความนี้จะอธิบายวิธีการเพิ่มหรือเปลี่ยนแปลงบทบาทผู้ดูแลระบบสำหรับผู้ใช้ที่ใช้ Azure RBAC ที่ขอบเขตการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="54043-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="54043-109">ใช้ PowerShell เพื่อเพิ่มเจ้าของกลุ่มหรือเจ้าของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="54043-109">Use PowerShell to add a group owner or an application owner.</span></span>
