---
title: ลบไซต์ SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/24/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c060815d-1d3f-4a13-81c2-0377bbeda202
ms.openlocfilehash: f6ee16a20f2280ba4d8d28ab3fdb4672cd9963b5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927595"
---
# <a name="delete-a-sharepoint-site"></a><span data-ttu-id="97b0c-102">ลบไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="97b0c-102">Delete a SharePoint site</span></span>
 <span data-ttu-id="97b0c-103">**ลบไซต์จากศูนย์ดูแล SharePoint ใหม่**</span><span class="sxs-lookup"><span data-stu-id="97b0c-103">**Delete sites from the new SharePoint admin center**</span></span>
  
<span data-ttu-id="97b0c-p101">เมื่อต้องการลบไซต์ที่มีการใช้งาน ไปที่ศูนย์กลางการดูแล SharePoint ปัจจุบัน คลิก "ลองใช้ได้เลย" ในมุมขวาด้านบน เลือก**ไซต์ที่ใช้งานอยู่**เลือกไซต์ จากนั้น**ลบ** เมื่อต้องการ[ดูและคืนค่าลบไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)เลือก**ลบไซต์** สำหรับข้อมูลเพิ่มเติม ให้ดู[จัดการไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center)</span><span class="sxs-lookup"><span data-stu-id="97b0c-p101">To delete an active site, go to the current SharePoint admin center, click "Try it now" in the upper right. Select **Active sites**, select the site, and then select **Delete**. To [view and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center), select **Deleted sites**. For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center).</span></span>
  
<span data-ttu-id="97b0c-p102">**สำคัญ:** ถ้าไซต์เป็นส่วนหนึ่งของนโยบายการเก็บข้อมูล คุณอาจไม่สามารถลบได้จนกว่าไซต์นั้นจะถูกเอาออกจากการ[ความปลอดภัย&amp;ศูนย์ดูแลการปฏิบัติตามกฎระเบียบ](https://protection.office.com/?rfr=AdminCenter#/homepage)ได้ ดู[ภาพรวมของนโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="97b0c-p102">**Important:** If the site is part of a retention policy, you may not be able to delete it until the site is removed from the [Security &amp; Compliance Admin Center](https://protection.office.com/?rfr=AdminCenter#/homepage). See [Overview of Retention Policies](https://docs.microsoft.com/office365/securitycompliance/retention-policies#content-in-onedrive-accounts-and-sharepoint-sites) for more info.</span></span> 
  
<span data-ttu-id="97b0c-110">เคล็ดลับ:</span><span class="sxs-lookup"><span data-stu-id="97b0c-110">Tips:</span></span>
- <span data-ttu-id="97b0c-p103">ผู้ดูแลส่วนกลางและผู้ดูแล SharePoint สามารถเดี๋ยวนี้ลบไซต์ที่อยู่ใน**Office 365 กลุ่ม** ดำเนินการนี้จะลบกลุ่มและทั้งหมดของทรัพยากร รวมถึงกล่องจดหมาย Outlook และปฏิทิน และทีมสถานีใด ๆ สำหรับข้อมูลเพิ่มเติม ดู[ลบไซต์ SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="97b0c-p103">Global admins and SharePoint admins can now delete sites that belong to an **Office 365 Group**. This will delete the group and all its resources, including the Outlook mailbox and calendar, and any Teams channels. For more info, see [Delete a SharePoint site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span></span>
- <span data-ttu-id="97b0c-p104">คุณสามารถกู้คืนไซต์ถูกลบสำหรับวัน 93 หมายเหตุว่า ต้องคืนค่าดัชนีกลุ่มถูกลบภายใน 30 วัน สำหรับข้อมูลเพิ่มเติม ดู[มุมมองและการคืนค่าไซต์ที่ถูกลบ](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center)</span><span class="sxs-lookup"><span data-stu-id="97b0c-p104">You can recover deleted sites for 93 days. Note that deleted groups must be restored within 30 days. For more info, see [View and restore deleted sites](https://docs.microsoft.com/sharepoint/view-and-restore-deleted-sites-in-new-admin-center).</span></span>
- <span data-ttu-id="97b0c-117">เมื่อต้องการเอาไซต์ ด้วย Powershell ดูตัวอย่างการ cmdlet [SPSite เอา](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="97b0c-117">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/powershell/module/sharepoint-server/remove-spsite?view=sharepoint-ps) cmdlet example.</span></span> 
  

