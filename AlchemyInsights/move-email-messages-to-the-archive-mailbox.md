---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747222"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="a5a50-102">ย้ายอีเมลไปยังกล่องจดหมายการเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="a5a50-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="a5a50-103">ยืนยันว่า การ**เก็บถาวรกล่องจดหมาย**ได้ถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="a5a50-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="a5a50-104">ถ้า ไม่มี ใช้ขั้นตอนต่าง ๆ ใน[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานการเก็บถาวรกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="a5a50-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="a5a50-105">จัดเก็บข้อความโดยอัตโนมัติไปยังกล่องจดหมายการเก็บถาวร แท็กเก็บข้อมูลที่ มีการดำเนินการ**ย้ายที่เก็บถาวร**ต้องถูกตั้งค่าเพื่อ**นำไปใช้กับแท็กกล่องจดหมายทั้งหมด (ค่าเริ่มต้น) โดยอัตโนมัติ**</span><span class="sxs-lookup"><span data-stu-id="a5a50-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="a5a50-106">ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กที่เก็บถาวรเริ่มต้น](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)</span><span class="sxs-lookup"><span data-stu-id="a5a50-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="a5a50-107">ถัดไป เพิ่มแท็ก**เก็บถาวร**นโยบายการเก็บข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5a50-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="a5a50-108">เลือก**นโยบายการเก็บข้อมูล**ในศูนย์ดูแล Exchange, > เพิ่มการ**ย้ายไปยังการเก็บถาวรแท็ก**> นโยบายการ**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="a5a50-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="a5a50-109">ขณะนี้[กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)กับกล่องจดหมายของผู้ใช้ที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="a5a50-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="a5a50-110">จะใช้นโยบายเดียวกันกับ**หลัก**และกล่องจดหมาย**เก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="a5a50-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="a5a50-111">คุณอาจจำเป็นในการบังคับใช้การจัดการโฟลเดอร์ผู้ช่วย (MFA) เมื่อต้องการเรียกใช้ และใช้การตั้งค่าใหม่กับกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a5a50-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="a5a50-112">เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ:</span><span class="sxs-lookup"><span data-stu-id="a5a50-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="a5a50-113">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ดู[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="a5a50-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

