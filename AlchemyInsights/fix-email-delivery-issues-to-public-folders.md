---
title: แก้ไขปัญหาการนําส่งอีเมลไปให้กับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716371"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="947c9-102">แก้ไขปัญหาการนําส่งอีเมลไปให้กับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย</span><span class="sxs-lookup"><span data-stu-id="947c9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="947c9-103">ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายของคุณ และผู้ส่งได้รับข้อผิดพลาด:**ไม่พบ (550 5.4.1)** ตรวจสอบว่าโดเมนอีเมลสําหรับโฟลเดอร์สาธารณะถูกกําหนดค่าเป็นโดเมนรีเลย์ภายในแทนโดเมนที่มีสิทธิ์:</span><span class="sxs-lookup"><span data-stu-id="947c9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="947c9-104">เปิด[ศูนย์การจัดการ Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="947c9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="947c9-105">ไปที่\>**โดเมนที่ยอมรับ\*\*\*\*ขั้นตอนจดหมาย**ให้เลือกโดเมนที่ยอมรับ แล้วคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="947c9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="947c9-106">ในเพจคุณสมบัติที่เปิดขึ้น**Authoritative\*\*\*\*Internal relay\*\*\*\*Save**</span><span class="sxs-lookup"><span data-stu-id="947c9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="947c9-107">ถ้าผู้ส่งภายนอกได้รับข้อผิดพลาด**ที่คุณไม่มีสิทธิ์ (550 5.7.13)** เรียกใช้คําสั่งต่อไปนี้ใน[PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เพื่อดูสิทธิ์สําหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:</span><span class="sxs-lookup"><span data-stu-id="947c9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="947c9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="947c9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="947c9-109">เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกส่งอีเมลไปยังโฟลเดอร์นี้สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="947c9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="947c9-110">ตัวอย่างเช่น`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="947c9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
