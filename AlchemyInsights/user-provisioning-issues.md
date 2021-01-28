---
title: ปัญหาการเตรียมใช้งานผู้ใช้
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
- "7762"
- "9004348"
ms.openlocfilehash: eed5886e5de391a203882f373f7ba8a71830b0d1
ms.sourcegitcommit: 28a79ef23c4a510397f4a8339ac2c5ff70eec713
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2021
ms.locfileid: "50036108"
---
# <a name="user-provisioning-issues"></a><span data-ttu-id="9e154-102">ปัญหาการเตรียมใช้งานผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="9e154-102">User-provisioning issues</span></span>

<span data-ttu-id="9e154-103">บทความนี้จะอธิบายวิธีการแก้ไขปัญหาที่คุณเผชิญอยู่ขณะเตรียมใช้งานผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="9e154-103">This article describes how to troubleshoot the issues you face when provisioning users.</span></span>

<span data-ttu-id="9e154-104">สําหรับคําแนะนําเมื่อพบปัญหาการเตรียมใช้งานผู้ใช้ต่างๆ ให้ปฏิบัติตามคําแนะนําด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="9e154-104">For guidance when encountering the various user-provisioning issues, follow the instructions below:</span></span>

1. <span data-ttu-id="9e154-105">คุณควรเริ่มต้นด้วยการค้นหาบทช่วยสอนการตั้งค่าเฉพาะในการตั้งค่าการเตรียมใช้งานแอปพลิเคชันของคุณเสมอ</span><span class="sxs-lookup"><span data-stu-id="9e154-105">You should always start by finding the setup tutorial specific to setting up provisioning for your application.</span></span> <span data-ttu-id="9e154-106">จากนั้นให้ปฏิบัติตามขั้นตอนเหล่านั้นเพื่อกําหนดค่าทั้งแอปและ Azure Active Directory (AD) เพื่อสร้างการเชื่อมต่อการเตรียมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="9e154-106">Then follow those steps to configure both the app and Azure Active Directory (AD) to create the provisioning connection.</span></span> <span data-ttu-id="9e154-107">สามารถดูรายการของบทช่วยสอนของแอปได้ที่[รายการบทช่วยสอนเกี่ยวกับวิธีการรวมแอป SaaS กับ Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)</span><span class="sxs-lookup"><span data-stu-id="9e154-107">A list of app tutorials can be found at [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).</span></span>
2. <span data-ttu-id="9e154-108">แก้ไขปัญหาการเตรียมใช้งานผู้ใช้โดยการอ้างถึงบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9e154-108">Troubleshoot the user-provisioning issues by referring to the following articles:</span></span>
    - <span data-ttu-id="9e154-109">[ปัญหาที่ทราบ](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues) แล้ว - ควรระวังเมื่อต้องใช้งานการเตรียมใช้งานแอป</span><span class="sxs-lookup"><span data-stu-id="9e154-109">[Known issues](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues) - To be aware of when working with app provisioning.</span></span>
    - <span data-ttu-id="9e154-110">[รายงานการเตรียมใช้งานใน](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) พอร์ทัล Azure Active Directory (ตัวอย่าง)</span><span class="sxs-lookup"><span data-stu-id="9e154-110">[Provisioning reports](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in the Azure Active Directory portal (preview)</span></span>
    - [<span data-ttu-id="9e154-111">ฉันไม่ทราบวิธีการกําหนดค่าการเตรียมใช้งานผู้ใช้ไปยังแอปพลิเคชันแกลเลอรี Azure AD</span><span class="sxs-lookup"><span data-stu-id="9e154-111">I don't know how to configure user provisioning to an Azure AD Gallery application</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/configure-automatic-user-provisioning-portal) 
    - [<span data-ttu-id="9e154-112">ฉันพบปัญหาเมื่อกําหนดค่าการเตรียมใช้งานผู้ใช้ไปยังแอปพลิเคชันแกลเลอรี Azure AD</span><span class="sxs-lookup"><span data-stu-id="9e154-112">I encountered a problem when configuring user provisioning to an Azure AD Gallery application</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem) 
    - [<span data-ttu-id="9e154-113">ฉันได้ตั้งค่าการเตรียมใช้งานแอปพลิเคชัน Azure AD Gallery ของฉัน แต่ไม่มีการเตรียมใช้งานผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="9e154-113">I've set up provisioning to my Azure AD Gallery application, but no users are being provisioned</span></span>](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned) 
    - [<span data-ttu-id="9e154-114">การเตรียมใช้งานแอปพลิเคชันแกลเลอรี Azure AD ของฉันใช้งานได้ แต่มีการเตรียมใช้งานชุดผู้ใช้ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="9e154-114">Provisioning to my Azure AD Gallery application is working, but the wrong set of users are being provisioned</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-assign-users)





