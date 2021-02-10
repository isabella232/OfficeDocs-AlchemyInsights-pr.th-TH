---
title: จัดการข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้
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
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177779"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="d4974-102">จัดการข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="d4974-103">การจัดการข้อมูลเฉพาะตัวที่มีการจัดการซึ่งผู้ใช้ได้รับมอบหมายนั้นเกี่ยวข้องกับ</span><span class="sxs-lookup"><span data-stu-id="d4974-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="d4974-104">การกําหนดบทบาทให้กับข้อมูลเฉพาะตัวที่มีการจัดการที่กําหนดโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="d4974-105">การลบข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="d4974-106">การแสดงข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="d4974-107">ดูข้อมูลเพิ่มเติมเกี่ยวกับงานที่ระบุไว้ด้านบนบทความต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="d4974-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="d4974-108">[วิธีสร้างข้อมูลเฉพาะตัวที่มีการจัดการที่กําหนดโดยผู้ใช้](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - การกําหนดบทบาทให้กับข้อมูลเฉพาะตัวที่มีการจัดการที่กําหนดโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="d4974-109">[วิธีการลบข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - เพื่อลบข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="d4974-110">[วิธีการแสดงรายการข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - แสดงรายการข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="d4974-111">ตรวจสอบว่าคุณมีการมอบหมาย **บทบาทที่มีการจัดการข้อมูลเฉพาะตัว** หรือไม่</span><span class="sxs-lookup"><span data-stu-id="d4974-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="d4974-112">การมอบหมายบทบาทนั้นจะต้องสร้าง/ลบข้อมูลเฉพาะตัวที่มีการจัดการที่มอบหมายโดยผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d4974-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
