---
title: การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707973"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="bd430-102">แก้ไขปัญหาการเข้าถึงข้อความที่ถูกปฏิเสธในศูนย์การจัดการ Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="bd430-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="bd430-103">ถ้าคุณได้รับข้อความปฏิเสธการเข้าถึงเมื่อพยายามเรียกดูศูนย์การจัดการ Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณได้กําหนด [สิทธิ์การใช้งานให้กับ](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="bd430-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="bd430-104">ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรตรวจสอบให้แน่ใจว่าพวกเขาได้รับมอบหมาย [บทบาทผู้ดูแลระบบ](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ที่สามารถเข้าถึงศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="bd430-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="bd430-105">ปัญหานี้ยังสามารถเกิดขึ้นเมื่อผู้ใช้ถูกลบและสร้างใหม่ด้วยชื่อหลักของผู้ใช้ (UPN) เดียวกัน</span><span class="sxs-lookup"><span data-stu-id="bd430-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="bd430-106">บัญชีใหม่จะถูกสร้างขึ้นโดยใช้รหัส PUID (รหัสพาสปอร์ตไม่ซ้ากัน) ค่าอื่น</span><span class="sxs-lookup"><span data-stu-id="bd430-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="bd430-107">เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="bd430-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="bd430-108">สถานการณ์ที่สองเกี่ยวข้องกับการซิงโครไนซ์ไดเรกทอรีด้วย Active Directory ขององค์กร (OU)</span><span class="sxs-lookup"><span data-stu-id="bd430-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="bd430-109">ถ้าผู้ใช้ลงชื่อเข้าใช้ SharePoint แล้วและถูกย้ายไปยัง OU อื่นและซิงค์กับ SharePoint อีกครั้ง ผู้ใช้อาจพบปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="bd430-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="bd430-110">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิมด้วยขั้นตอนในบทความ คืนค่า[ผู้ใช้ใน Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="bd430-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="bd430-111">หมายเหตุ: ถ้าศูนย์การจัดการ OneDrive หรือ SharePoint ไม่พร้อมใช้งานกับผู้ใช้หลายรายที่เคยมีสิทธิ์เข้าถึง อาจมีปัญหาด้านบริการชั่วคราว</span><span class="sxs-lookup"><span data-stu-id="bd430-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="bd430-112">[ตรวจสอบแดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="bd430-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


