---
title: แก้ไขปัญหาการนำส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677947"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="74e98-102">แก้ไขปัญหาการนำส่งอีเมลไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย</span><span class="sxs-lookup"><span data-stu-id="74e98-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="74e98-103">ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายของคุณได้และผู้ส่งได้รับข้อผิดพลาด: ไม่ **พบ (๕๕๐ 5.4.1)** ตรวจสอบโดเมนอีเมลสำหรับโฟลเดอร์สาธารณะที่ได้รับการกำหนดค่าเป็นโดเมน relay ภายในแทนที่จะเป็นโดเมนที่มีสิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="74e98-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="74e98-104">เปิด[ศูนย์การจัดการ Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="74e98-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="74e98-105">ไปที่**Mail flow** \> **โดเมนที่ยอมรับ**จดหมายเวียนให้เลือกโดเมนที่ยอมรับแล้วคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="74e98-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="74e98-106">ในหน้าคุณสมบัติที่เปิดขึ้นถ้ามีการตั้งค่าชนิดโดเมนเป็น**สิทธิ์**ให้เปลี่ยนค่าเป็น**รีเลย์ภายใน**แล้วคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="74e98-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="74e98-107">ถ้าผู้ส่งภายนอกได้รับข้อผิดพลาดที่ **คุณไม่มีสิทธิ์ (๕๕๐ 5.7.13)** ให้เรียกใช้คำสั่งต่อไปนี้ใน [PowerShell Online Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) เพื่อดูสิทธิ์สำหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:</span><span class="sxs-lookup"><span data-stu-id="74e98-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="74e98-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` ตัว `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` อย่างเช่น</span><span class="sxs-lookup"><span data-stu-id="74e98-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="74e98-109">เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกส่งอีเมลไปยังโฟลเดอร์สาธารณะนี้ให้เพิ่มการเข้าถึง CreateItems ขวาไปยังผู้ใช้ที่ไม่ระบุชื่อ</span><span class="sxs-lookup"><span data-stu-id="74e98-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="74e98-110">ตัว `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` อย่างเช่น</span><span class="sxs-lookup"><span data-stu-id="74e98-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
