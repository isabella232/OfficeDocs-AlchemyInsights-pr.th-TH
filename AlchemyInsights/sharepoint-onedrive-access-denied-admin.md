---
title: การแก้ปัญหาข้อความการเข้าถึงถูกปฏิเสธ
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051444"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="f1118-102">การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์การจัดการ Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1118-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="f1118-103">ถ้าคุณได้รับข้อความที่ถูกปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูไปยังศูนย์ดูแล Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้[กำหนดสิทธิ์การใช้งานให้กับ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="f1118-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="f1118-104">ถ้าผู้ใช้มีใบอนุญาตคุณควรตรวจสอบให้แน่ใจว่ามี[การกำหนดบทบาทผู้ดูแลระบบ](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)ที่สามารถเข้าถึงศูนย์ดูแล</span><span class="sxs-lookup"><span data-stu-id="f1118-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="f1118-105">ปัญหานี้อาจเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างขึ้นใหม่ด้วยชื่อผู้ใช้หลักเดียวกัน (UPN)</span><span class="sxs-lookup"><span data-stu-id="f1118-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f1118-106">บัญชีใหม่จะถูกสร้างขึ้นโดยใช้ค่า PUID (รหัสเฉพาะที่ไม่ซ้ำกัน)</span><span class="sxs-lookup"><span data-stu-id="f1118-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f1118-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขาผู้ใช้มี PUID ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f1118-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f1118-108">สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนส์ของไดเรกทอรีกับหน่วยองค์กรไดเรกทอรีที่ใช้งานอยู่ (OU)</span><span class="sxs-lookup"><span data-stu-id="f1118-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f1118-109">ถ้าผู้ใช้มีการลงชื่อเข้าสู่ SharePoint แล้วและถูกย้ายไปยัง OU ที่แตกต่างกันและทำซ้ำกับ SharePoint พวกเขาอาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="f1118-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="f1118-110">เพื่อแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ[คืนค่าผู้ใช้ใน Office ๓๖๕](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f1118-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="f1118-111">หมายเหตุ: ถ้าการ OneDrive หรือศูนย์กลางการดูแล SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่ก่อนหน้านี้มีการเข้าถึงอาจมีปัญหาการบริการแบบถาวร</span><span class="sxs-lookup"><span data-stu-id="f1118-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="f1118-112">[ตรวจสอบแดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="f1118-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


