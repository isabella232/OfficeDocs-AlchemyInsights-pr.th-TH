---
title: ลบไซต์กลุ่ม
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "567"
- "5200006"
ms.assetid: aa6c2aa1-6853-461c-8764-01fb96f8e981
ms.openlocfilehash: 6087240b0615d4d0d6fcfdbbb77fdc15dbafd289
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745842"
---
# <a name="delete-a-sharepoint-site-that-belongs-to-a-microsoft-365-group"></a><span data-ttu-id="63961-102">ลบไซต์ SharePoint ที่เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="63961-102">Delete a SharePoint site that belongs to a Microsoft 365 group</span></span>

<span data-ttu-id="63961-103">การลบไซต์ที่เชื่อมต่อกับกลุ่มจะเป็นการลบกลุ่มและทรัพยากรทั้งหมดรวมถึงกล่องจดหมายและปฏิทินของ Outlook และแชนเนลของทีมใดก็ตาม</span><span class="sxs-lookup"><span data-stu-id="63961-103">Deleting a group-connected site will delete the group and all its resources, including the Outlook mailbox and calendar, and any Teams channels.</span></span>
  
<span data-ttu-id="63961-104">สำคัญ</span><span class="sxs-lookup"><span data-stu-id="63961-104">Important:</span></span>

- <span data-ttu-id="63961-105">คุณสามารถกู้คืนไซต์ที่ถูกลบสำหรับ๙๓วันได้</span><span class="sxs-lookup"><span data-stu-id="63961-105">You can recover deleted sites for 93 days.</span></span> <span data-ttu-id="63961-106">กลุ่มที่ถูกลบจะต้องได้รับการคืนค่าภายใน30วัน</span><span class="sxs-lookup"><span data-stu-id="63961-106">Deleted groups must be restored within 30 days.</span></span> <span data-ttu-id="63961-107">[ดูและคืนค่าไซต์ที่ถูกลบ](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) โดยตรงจากศูนย์การจัดการ SharePoint</span><span class="sxs-lookup"><span data-stu-id="63961-107">[View and restore deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) directly from the SharePoint Admin Center.</span></span> <span data-ttu-id="63961-108">เมื่อต้องการ[ดูและคืนค่า**กลุ่มที่ถูกลบ**](https://outlook.office.com/people/group/deleted)ให้เลือก**จัดการกลุ่ม**จากนั้นเลือก**ลบ**</span><span class="sxs-lookup"><span data-stu-id="63961-108">To [view and restore **deleted groups**](https://outlook.office.com/people/group/deleted), select **Manage Groups**, then choose **Deleted**.</span></span>
- <span data-ttu-id="63961-109">ถ้าไซต์เป็นส่วนหนึ่งของนโยบายการเก็บข้อมูลคุณอาจไม่สามารถลบไซต์ดังกล่าวได้จนกว่าไซต์จะถูกเอาออกจาก[ศูนย์การจัดการการรักษาความปลอดภัย & การปฏิบัติตามนโยบาย](https://protection.office.com/?rfr=AdminCenter#/retention)</span><span class="sxs-lookup"><span data-stu-id="63961-109">If the site is part of a retention policy, you may not be able to delete it until the site is removed from the [Security & Compliance Admin Center](https://protection.office.com/?rfr=AdminCenter#/retention).</span></span> <span data-ttu-id="63961-110">สำหรับข้อมูลเพิ่มเติมให้ดู[ภาพรวมของนโยบายการเก็บข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)</span><span class="sxs-lookup"><span data-stu-id="63961-110">For more info, see the [Overview of Retention Policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>
  
<span data-ttu-id="63961-111">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการไซต์ในศูนย์การจัดการ SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center)</span><span class="sxs-lookup"><span data-stu-id="63961-111">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span></span>
