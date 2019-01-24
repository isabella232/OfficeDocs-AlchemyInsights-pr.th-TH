---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493509"
---
<span data-ttu-id="6e1ef-p101">มีปัญหาในการเก็บถาวรรายการไปยังกล่องจดหมายการเก็บถาวร ตรวจสอบให้แน่ใจว่า คุณได้ดำเนินการขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="6e1ef-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="6e1ef-p102">ยืนยันว่า การ**เก็บถาวรกล่องจดหมาย**ได้ถูกเปิดใช้งาน ถ้า ไม่มี ทำตามขั้นตอนใน[บทความนี้](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานการเก็บถาวรกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="6e1ef-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="6e1ef-106">ในศูนย์ดูแล Exchange เลือก**แท็กการเก็บข้อมูล**ที่อยู่ภายใต้การ**บริหารการปฏิบัติตามกฎระเบียบ**สร้าง**แท็กการเก็บข้อมูล**ที่ มีการดำเนินการ**ย้ายไปยังที่เก็บถาวร**ที่ประกอบด้วย**อายุการเก็บข้อมูล**ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="6e1ef-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="6e1ef-107">ในศูนย์ดูแล Exchange เลือก**นโยบายการเก็บข้อมูล**สร้าง**นโยบายการเก็บข้อมูล**และเพิ่มแท็กเก็บข้อมูลของคุณ**ย้ายไปยังที่เก็บถาวร**ที่นโยบาย</span><span class="sxs-lookup"><span data-stu-id="6e1ef-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="6e1ef-p103">[กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)กับกล่องจดหมายของผู้ใช้ที่ระบุ จะใช้นโยบายเดียวกันกับ**หลัก**และกล่องจดหมาย**เก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="6e1ef-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="6e1ef-p104">กล่องจดหมายของผู้ใช้ควรมีมีนโยบายการเก็บถาวรเพื่อย้ายรายการไปยังกล่องจดหมายการเก็บถาวรในขณะนี้ คุณอาจจำเป็นในการบังคับใช้การจัดการโฟลเดอร์ผู้ช่วย (MFA) เมื่อต้องการเรียกใช้ และใช้การตั้งค่าใหม่กับกล่องจดหมายของผู้ใช้ เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ:</span><span class="sxs-lookup"><span data-stu-id="6e1ef-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="6e1ef-113">ต้องการข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ดูการ[ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="6e1ef-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

