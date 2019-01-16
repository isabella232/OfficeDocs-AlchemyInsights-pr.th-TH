---
title: นโยบายการเก็บข้อมูลในศูนย์ดูแล Exchange ไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316079"
---
 <span data-ttu-id="13292-102">**ปัญหา:** สร้างใหม่ หรือนโยบายการเก็บข้อมูลที่ปรับปรุงแล้วในศูนย์ดูแล Exchange จะไม่นำไปใช้กับกล่องจดหมาย หรือรายการถูกย้ายไปยังกล่องจดหมายการเก็บถาวร หรือถูกลบ</span><span class="sxs-lookup"><span data-stu-id="13292-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="13292-103">**สาเหตุราก:**</span><span class="sxs-lookup"><span data-stu-id="13292-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="13292-p101">ซึ่งอาจเนื่องมาจากผู้**จัดการผู้ช่วยของโฟลเดอร์**ยังไม่ประมวลผลกล่องจดหมายของผู้ใช้ ผู้จัดการโฟลเดอร์ช่วยพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรของคุณใช้ cloud ทุก ๆ 7 วันครั้งเดียว ถ้าคุณเปลี่ยนแปลงแท็กเก็บข้อมูล หรือใช้นโยบายการเก็บข้อมูลที่แตกต่างกันไปยังกล่องจดหมาย คุณสามารถรอจนกระทั่งการจัดการโฟลเดอร์ช่วยประมวลผลกล่องจดหมาย หรือคุณสามารถเรียกใช้ cmdlet ManagedFolderAssistant เริ่มต้นเพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยในการประมวลผลเฉพาะ กล่องจดหมาย เรียกใช้ cmdlet นี้จะเป็นประโยชน์สำหรับการทดสอบ หรือการแก้ไขปัญหานโยบายการเก็บข้อมูลหรือการตั้งค่าแท็กการเก็บข้อมูล สำหรับข้อมูลเพิ่มเติม โปรดเยี่ยมชมที่[เรียกใช้การจัดการโฟลเดอร์ผู้ช่วย](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)</span><span class="sxs-lookup"><span data-stu-id="13292-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="13292-109">**โซลูชัน:** เรียกใช้คำสั่งต่อไปนี้เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ:</span><span class="sxs-lookup"><span data-stu-id="13292-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="13292-p102">ซึ่งอาจจะเกิดขึ้น**RetentionHold**ถูก**เปิดใช้งาน**ในกล่องจดหมาย ถ้ากล่องจดหมายที่ถูกวางไว้บน RetentionHold นโยบายการเก็บข้อมูลในกล่องจดหมายจะไม่สามารถดำเนินการในระหว่างเวลานั้น สำหรับ informaton เพิ่มเติมในการดูการตั้งค่า RetentionHold:[เก็บข้อมูลกล่องจดหมายที่เก็บ](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="13292-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="13292-113">**โซลูชัน:**</span><span class="sxs-lookup"><span data-stu-id="13292-113">**Solution:**</span></span>
    
  - <span data-ttu-id="13292-114">ตรวจสอบสถานะของการตั้งค่ากล่องจดหมายเฉพาะเจาะจงใน[EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="13292-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="13292-115">เรียกใช้คำสั่งต่อไปนี้เพื่อ**ปิดการใช้งาน**RetentionHold บนกล่องจดหมายเฉพาะ:</span><span class="sxs-lookup"><span data-stu-id="13292-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="13292-116">ขณะนี้ เรียกใช้ใหม่ในโฟลเดอร์ที่มีการจัดการผู้ช่วย:</span><span class="sxs-lookup"><span data-stu-id="13292-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="13292-117">**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 เมกะไบต์ ผู้จัดการโฟลเดอร์ช่วยจะไม่ประมวลผลโดยอัตโนมัติกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="13292-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

