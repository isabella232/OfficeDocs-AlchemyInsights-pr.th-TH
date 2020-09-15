---
title: เพิ่มเอาออกหรือป้องกันไม่ให้ผู้ใช้เปลี่ยนรูปโปรไฟล์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001499"
- "3552"
ms.openlocfilehash: 58b428e3110c06b8b39d45d327ac514c4245be81
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687813"
---
# <a name="add-remove-or-prevent-users-from-changing-profile-photos"></a><span data-ttu-id="41e2a-102">เพิ่มเอาออกหรือป้องกันไม่ให้ผู้ใช้เปลี่ยนรูปโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="41e2a-102">Add, remove, or prevent users from changing profile photos</span></span>

- <span data-ttu-id="41e2a-103">การ**เพิ่มรูปถ่ายโปรไฟล์:** รูปภาพโปรไฟล์สามารถเพิ่มได้โดยผู้ดูแลระบบใน[ศูนย์การจัดการ Microsoft ๓๖๕ผู้ใช้ที่ใช้งานอยู่](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)หรือ[การจัดการผู้ใช้ Active directory ของ Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers)</span><span class="sxs-lookup"><span data-stu-id="41e2a-103">**Adding profile photos:** Profile photos can be added by an administrator in [Microsoft 365 admin center, Active users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) or  [Azure Active Directory User Management](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers).</span></span>  <span data-ttu-id="41e2a-104">ถ้าคุณไม่เห็นตัวเลือก "เปลี่ยนรูปภาพ" ให้ตรวจสอบให้แน่ใจว่ามีการกำหนดสิทธิ์การใช้งานให้กับผู้ใช้รายนั้น</span><span class="sxs-lookup"><span data-stu-id="41e2a-104">If you don't see the "change photo" option, be sure a license is assigned to that user.</span></span> <span data-ttu-id="41e2a-105">รูปถ่ายสามารถเพิ่มหรือเปลี่ยนแปลงโดยผู้ใช้ในโปรไฟล์ผู้ใช้ของพวกเขาจากบริการ Microsoft ๓๖๕ได้โดยการคลิกชื่อย่อ/รูปถ่ายของพวกเขาที่ด้านขวาบนของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="41e2a-105">Photos can be added or changed by a user in their user profile from any Microsoft 365 service by clicking their initials / photo in the upper right of the screen.</span></span> <span data-ttu-id="41e2a-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเพิ่มรูปถ่ายโปรไฟล์ให้ดูที่[เพิ่มรูปภาพโปรไฟล์ของคุณไปยัง Microsoft ๓๖๕](https://support.office.com/article/add-your-profile-photo-to-office-365-2eaf93fd-b3f1-43b9-9cdc-bdcd548435b7)</span><span class="sxs-lookup"><span data-stu-id="41e2a-106">For more information on adding a profile photo, see [Add your profile photo to Microsoft 365](https://support.office.com/article/add-your-profile-photo-to-office-365-2eaf93fd-b3f1-43b9-9cdc-bdcd548435b7).</span></span>

- <span data-ttu-id="41e2a-107">การ**เอารูปภาพโปรไฟล์ออก:** รูปภาพโปรไฟล์สามารถเอาออกโดยผู้ดูแลระบบใน[Azure active Directory การจัดการผู้ใช้](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers)หรือโดยผู้ใช้ในโปรไฟล์ผู้ใช้ของ Microsoft team ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="41e2a-107">**Removing profile photos:** Profile photos can be removed by an administrator in [Azure Active Directory User Management](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers) or by a user in their Microsoft Teams user profile.</span></span>

- <span data-ttu-id="41e2a-108">**การบล็อกการเปลี่ยนแปลงรูปถ่ายของโปรไฟล์:** การเปลี่ยนแปลงรูปถ่ายอาจถูกบล็อกสำหรับ Microsoft ๓๖๕ \* โดยการเพิ่มนโยบาย Outlook Web App ต่อบทความการ[ล็อกรูปถ่ายหรือการจำกัดสิทธิ์ในการเปลี่ยนรูปโปรไฟล์ของ microsoft ๓๖๕](https://answers.microsoft.com/msoffice/forum/msoffice_o365admin-mso_manage/locking-photos-or-restricting-permissions-to/1d19ae4f-de5d-4c3d-a0ad-4b8b8ac32e3d)</span><span class="sxs-lookup"><span data-stu-id="41e2a-108">**Blocking profile photo changes:** Photo changes can be blocked for all of Microsoft 365\* by adding an Outlook Web App policy per the article, [Locking photos or restricting permissions to change Microsoft 365 profile photo](https://answers.microsoft.com/msoffice/forum/msoffice_o365admin-mso_manage/locking-photos-or-restricting-permissions-to/1d19ae4f-de5d-4c3d-a0ad-4b8b8ac32e3d).</span></span>

<span data-ttu-id="41e2a-109">\* โปรดทราบว่าทีม Microsoft ไม่สนับสนุนนโยบาย Outlook Web App ในขณะนี้เพื่อบล็อกการเปลี่ยนแปลงรูปภาพแต่กำลังวางแผนที่จะเพิ่มการสนับสนุนสำหรับฟีเจอร์นี้ในช่วงต้น๒๐๒๐</span><span class="sxs-lookup"><span data-stu-id="41e2a-109">\*Please note that Microsoft Teams does not currently support the Outlook Web App policy to block photo changes but is planning to add support for this feature in early 2020.</span></span>
