---
title: แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387724"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="38acb-102">แก้ไขปัญหาการส่งอีเมลไปยังโฟลเดอร์สาธารณะที่ใช้จดหมาย</span><span class="sxs-lookup"><span data-stu-id="38acb-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="38acb-103">ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะของคุณเปิดใช้งานจดหมาย และรายชื่อผู้ส่งที่ได้รับข้อผิดพลาด:**ไม่พบ (550 5.4.1)**, ตรวจสอบโดเมนอีเมลสำหรับโฟลเดอร์สาธารณะที่ถูกกำหนดค่าเป็นโดเมนรีเลย์ภายในที่แทน โดเมนที่เชื่อถือได้:</span><span class="sxs-lookup"><span data-stu-id="38acb-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="38acb-104">เปิด[ศูนย์ดูแล Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="38acb-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="38acb-105">**การรับส่งจดหมาย**ไป\>**โดเมน Accepted**เลือกโดเมนยอมรับได้ และจากนั้น คลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="38acb-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="38acb-106">ในคุณสมบัติของหน้านั้นเปิด ถ้าชนิดโดเมนถูกตั้งค่าเป็น**Authoritative**เปลี่ยนค่าเป็น**สับเปลี่ยนภายใน**และจากนั้น คลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="38acb-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="38acb-107">หากผู้ส่งภายนอกได้รับการข้อผิดพลาด**คุณไม่ได้รับอนุญาต (550 5.7.13)**, เรียกใช้คำสั่งต่อไปนี้ใน[PowerShell ออนไลน์ของ Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เมื่อต้องการดูสิทธิ์สำหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:</span><span class="sxs-lookup"><span data-stu-id="38acb-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="38acb-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`</span><span class="sxs-lookup"><span data-stu-id="38acb-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="38acb-109">เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกเพื่อส่งอีเมลไปที่โฟลเดอร์สาธารณะนี้ เพิ่มการเข้าถึง CreateItems ขวาไปผู้ใช้ที่ไม่ระบุชื่อ</span><span class="sxs-lookup"><span data-stu-id="38acb-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="38acb-110">ตัวอย่างเช่น`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`</span><span class="sxs-lookup"><span data-stu-id="38acb-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
