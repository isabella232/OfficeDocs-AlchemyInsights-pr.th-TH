---
title: เพิ่ม เอาออก หรือป้องกันไม่ให้ผู้ใช้เปลี่ยนรูปภาพโปรไฟล์
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001499"
- "3552"
ms.openlocfilehash: 71c959da8d74a282023f9fbacf14dc4305ed708e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822402"
---
# <a name="add-remove-or-prevent-users-from-changing-profile-photos"></a><span data-ttu-id="cc526-102">เพิ่ม เอาออก หรือป้องกันไม่ให้ผู้ใช้เปลี่ยนรูปภาพโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="cc526-102">Add, remove, or prevent users from changing profile photos</span></span>

- <span data-ttu-id="cc526-103">**การเพิ่มรูปภาพโปรไฟล์:** รูปภาพโปรไฟล์สามารถเพิ่มได้โดยผู้ดูแลระบบในศูนย์การจัดการ [Microsoft 365 ผู้ใช้ที่ใช้งานอยู่](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) หรือ  [การจัดการ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers)ผู้ใช้ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cc526-103">**Adding profile photos:** Profile photos can be added by an administrator in [Microsoft 365 admin center, Active users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) or  [Azure Active Directory User Management](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers).</span></span>  <span data-ttu-id="cc526-104">ถ้าคุณไม่เห็นตัวเลือก "เปลี่ยนรูปภาพ" ให้ตรวจสอบให้แน่ใจว่าได้มอบหมายสิทธิ์การใช้งานให้กับผู้ใช้รายนั้นแล้ว</span><span class="sxs-lookup"><span data-stu-id="cc526-104">If you don't see the "change photo" option, be sure a license is assigned to that user.</span></span> <span data-ttu-id="cc526-105">ผู้ใช้สามารถเพิ่มหรือเปลี่ยนแปลงรูปถ่ายในโปรไฟล์ผู้ใช้จากบริการ Microsoft 365 ใดๆ โดยคลิกที่ชื่อย่อ / รูปภาพของพวกเขาที่มุมขวาบนของหน้าจอ</span><span class="sxs-lookup"><span data-stu-id="cc526-105">Photos can be added or changed by a user in their user profile from any Microsoft 365 service by clicking their initials / photo in the upper right of the screen.</span></span> <span data-ttu-id="cc526-106">For more information on adding a profile photo, see [Add your profile photo to Microsoft 365](https://support.office.com/article/add-your-profile-photo-to-office-365-2eaf93fd-b3f1-43b9-9cdc-bdcd548435b7).</span><span class="sxs-lookup"><span data-stu-id="cc526-106">For more information on adding a profile photo, see [Add your profile photo to Microsoft 365](https://support.office.com/article/add-your-profile-photo-to-office-365-2eaf93fd-b3f1-43b9-9cdc-bdcd548435b7).</span></span>

- <span data-ttu-id="cc526-107">**การเอารูปโปรไฟล์ออก:** รูปภาพโปรไฟล์สามารถลบออกได้โดยผู้ดูแลระบบในการจัดการผู้ใช้ [Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers) หรือโดยผู้ใช้ในโปรไฟล์ผู้ใช้ Microsoft Teams ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="cc526-107">**Removing profile photos:** Profile photos can be removed by an administrator in [Azure Active Directory User Management](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers) or by a user in their Microsoft Teams user profile.</span></span>

- <span data-ttu-id="cc526-108">**การบล็อกการเปลี่ยนแปลงรูปภาพโปรไฟล์:** การเปลี่ยนแปลงรูปภาพสามารถถูกบล็อกได้กับ Microsoft 365\* ทั้งหมด โดยการเพิ่มนโยบาย Outlook Web App ต่อบทความ การล็อกรูปภาพ หรือการจํากัดสิทธิ์เพื่อเปลี่ยนรูปภาพโปรไฟล์ [Microsoft 365](https://answers.microsoft.com/msoffice/forum/msoffice_o365admin-mso_dep365-mso_o365b/locking-photos-or-restricting-permissions-to/1d19ae4f-de5d-4c3d-a0ad-4b8b8ac32e3d)</span><span class="sxs-lookup"><span data-stu-id="cc526-108">**Blocking profile photo changes:** Photo changes can be blocked for all of Microsoft 365\* by adding an Outlook Web App policy per the article, [Locking photos or restricting permissions to change Microsoft 365 profile photo](https://answers.microsoft.com/msoffice/forum/msoffice_o365admin-mso_dep365-mso_o365b/locking-photos-or-restricting-permissions-to/1d19ae4f-de5d-4c3d-a0ad-4b8b8ac32e3d).</span></span>

<span data-ttu-id="cc526-109">\*ขณะนี้ Microsoft Teams ยังไม่สนับสนุนนโยบาย Outlook Web App เพื่อบล็อกการเปลี่ยนแปลงรูปภาพ แต่วางแผนที่จะเพิ่มการสนับสนุนฟีเจอร์นี้ในช่วงต้นปี 2020</span><span class="sxs-lookup"><span data-stu-id="cc526-109">\*Microsoft Teams does not currently support the Outlook Web App policy to block photo changes but is planning to add support for this feature in early 2020.</span></span>
