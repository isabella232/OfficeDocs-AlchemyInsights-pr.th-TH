---
title: ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715230"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="9528d-102">ให้ผู้ใช้สามารถเข้าถึง SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="9528d-102">Give users access to SharePoint and OneDrive</span></span>

<p><span data-ttu-id="9528d-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ปัญหานี้เกิดขึ้นบ่อยที่สุดเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN) สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU) ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span></span><span class="sxs-lookup"><span data-stu-id="9528d-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN). The new account is created by using a different PUID (Passport Unique ID) value. When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. A second scenario involves directory synchronization with an Active Directory organizational unit (OU). If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span></span></p> <p><span data-ttu-id="9528d-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">เมื่อต้องการแก้ไขปัญหานี้คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">คืนค่าผู้ใช้ใน Office 365</a></span></span><span class="sxs-lookup"><span data-stu-id="9528d-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">To resolve this issue you should restore the original UPN with the steps in the article, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Restore a user in Office 365.</a></span></span></span></p> <p><span data-ttu-id="9528d-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">หลังจากทำเช่นนี้ คุณสามารถตรวจสอบผู้ใช้มีสิทธิ์การดูแลไปยังไซต์ OneDrive โดยทำตามขั้นตอนในการ<a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">เพิ่มของผู้ดูแลระบบสำหรับ OneDrive ของผู้ใช้ได้</a></span></span><span class="sxs-lookup"><span data-stu-id="9528d-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Add admin's for a user's OneDrive.</a></span></span></span></p> <p><span data-ttu-id="9528d-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับระดับสิทธิ์ ให้ดูที่บทความ<a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">ทำความเข้าใจเกี่ยวกับระดับสิทธิ์ใน SharePoint</a>&nbsp;</span></span><span class="sxs-lookup"><span data-stu-id="9528d-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on permission levels, see the article, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">Understanding permission levels in SharePoint.</a>&nbsp;</span></span></span></p>
