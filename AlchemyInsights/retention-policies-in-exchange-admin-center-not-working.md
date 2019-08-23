---
title: นโยบายการเก็บข้อมูลในศูนย์ดูแล Exchange ไม่ทำงาน
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551362"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4690e-102">นโยบายการเก็บข้อมูลในศูนย์ดูแลอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="4690e-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="4690e-103">**ปัญหา:** สร้างใหม่ หรือนโยบายการเก็บข้อมูลที่ปรับปรุงแล้วในศูนย์ดูแล Exchange จะไม่นำไปใช้กับกล่องจดหมาย หรือรายการถูกย้ายไปยังกล่องจดหมายการเก็บถาวร หรือถูกลบ</span><span class="sxs-lookup"><span data-stu-id="4690e-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="4690e-104">**สาเหตุราก:**</span><span class="sxs-lookup"><span data-stu-id="4690e-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="4690e-105">ซึ่งอาจเนื่องมาจากผู้**จัดการผู้ช่วยของโฟลเดอร์**ยังไม่ประมวลผลกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="4690e-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4690e-106">ผู้จัดการโฟลเดอร์ช่วยพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรของคุณใช้ cloud ทุก ๆ 7 วันครั้งเดียว</span><span class="sxs-lookup"><span data-stu-id="4690e-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="4690e-107">ถ้าคุณเปลี่ยนแปลงแท็กเก็บข้อมูล หรือใช้นโยบายการเก็บข้อมูลที่แตกต่างกันไปยังกล่องจดหมาย คุณสามารถรอจนกระทั่งการจัดการโฟลเดอร์ช่วยประมวลผลกล่องจดหมาย หรือคุณสามารถเรียกใช้ cmdlet ManagedFolderAssistant เริ่มต้นเพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยในการประมวลผลเฉพาะ กล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4690e-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="4690e-108">เรียกใช้ cmdlet นี้จะเป็นประโยชน์สำหรับการทดสอบ หรือการแก้ไขปัญหานโยบายการเก็บข้อมูลหรือการตั้งค่าแท็กการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4690e-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="4690e-109">สำหรับข้อมูลเพิ่มเติม โปรดเยี่ยมชมที่[เรียกใช้การจัดการโฟลเดอร์ผู้ช่วย](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)</span><span class="sxs-lookup"><span data-stu-id="4690e-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="4690e-110">**โซลูชัน:** เรียกใช้คำสั่งต่อไปนี้เพื่อเริ่มต้นการจัดการโฟลเดอร์ผู้ช่วยสำหรับกล่องจดหมายระบุ:</span><span class="sxs-lookup"><span data-stu-id="4690e-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="4690e-111">ซึ่งอาจจะเกิดขึ้น**RetentionHold**ถูก**เปิดใช้งาน**ในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4690e-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4690e-112">ถ้ากล่องจดหมายที่ถูกวางไว้บน RetentionHold นโยบายการเก็บข้อมูลในกล่องจดหมายจะไม่สามารถดำเนินการในระหว่างเวลานั้น</span><span class="sxs-lookup"><span data-stu-id="4690e-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="4690e-113">สำหรับ informaton เพิ่มเติมในการดูการตั้งค่า RetentionHold:[เก็บข้อมูลกล่องจดหมายที่เก็บ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="4690e-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="4690e-114">**โซลูชัน:**</span><span class="sxs-lookup"><span data-stu-id="4690e-114">**Solution:**</span></span>
    
  - <span data-ttu-id="4690e-115">ตรวจสอบสถานะของการตั้งค่ากล่องจดหมายเฉพาะเจาะจงใน[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="4690e-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="4690e-116">เรียกใช้คำสั่งต่อไปนี้เพื่อ**ปิดการใช้งาน**RetentionHold บนกล่องจดหมายเฉพาะ:</span><span class="sxs-lookup"><span data-stu-id="4690e-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="4690e-117">ขณะนี้ เรียกใช้ใหม่ในโฟลเดอร์ที่มีการจัดการผู้ช่วย:</span><span class="sxs-lookup"><span data-stu-id="4690e-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="4690e-118">**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 เมกะไบต์ ผู้จัดการโฟลเดอร์ช่วยจะไม่ประมวลผลโดยอัตโนมัติกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4690e-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4690e-119">สำหรับข้อมูลเพิ่มเติมในนโยบายการเก็บข้อมูลในศูนย์ดูแลอัตราแลกเปลี่ยน ดู:</span><span class="sxs-lookup"><span data-stu-id="4690e-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="4690e-120">แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4690e-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="4690e-121">ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4690e-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="4690e-122">เพิ่ม หรือเอาแท็กการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4690e-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="4690e-123">วิธีการระบุชนิดของการระงับที่วางอยู่บนกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="4690e-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
