---
title: นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ไม่ทำงาน
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740529"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8b06d-102">นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange</span><span class="sxs-lookup"><span data-stu-id="8b06d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8b06d-103">ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหาเกี่ยวกับนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="8b06d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="8b06d-104">**ปัญหา:** นโยบายการเก็บข้อมูลที่สร้างขึ้นใหม่หรือที่อัปเดตในศูนย์การจัดการ Exchange จะไม่ถูกนำไปใช้กับกล่องจดหมายหรือรายการจะไม่ถูกย้ายไปยังกล่องจดหมายเก็บถาวรหรือถูกลบ</span><span class="sxs-lookup"><span data-stu-id="8b06d-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8b06d-105">**สาเหตุราก:**</span><span class="sxs-lookup"><span data-stu-id="8b06d-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="8b06d-106">ซึ่งอาจเป็นเพราะ **ผู้ช่วยโฟลเดอร์** ที่มีการจัดการยังไม่ได้ประมวลผลกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="8b06d-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8b06d-107">ผู้ช่วยโฟลเดอร์ที่ได้รับการจัดการพยายามดำเนินการทุกกล่องจดหมายในองค์กร cloud-based ของคุณทุกๆ7วัน</span><span class="sxs-lookup"><span data-stu-id="8b06d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="8b06d-108">ถ้าคุณเปลี่ยนแท็กการเก็บข้อมูลหรือนำนโยบายการเก็บข้อมูลอื่นไปใช้กับกล่องจดหมายคุณสามารถรอจนกว่าโฟลเดอร์ที่ได้รับการจัดการช่วยประมวลผลกล่องจดหมายหรือคุณสามารถเรียกใช้ cmdlet เริ่มต้น ManagedFolderAssistant เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการเพื่อประมวลผลกล่องจดหมายที่เฉพาะเจาะจงได้</span><span class="sxs-lookup"><span data-stu-id="8b06d-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="8b06d-109">การเรียกใช้ cmdlet นี้มีประโยชน์สำหรับการทดสอบหรือการแก้ไขปัญหานโยบายการเก็บข้อมูลหรือการตั้งค่าแท็กการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="8b06d-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="8b06d-110">สำหรับข้อมูลเพิ่มเติมให้เยี่ยมชม[เรียกใช้ตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการ](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)</span><span class="sxs-lookup"><span data-stu-id="8b06d-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8b06d-111">**วิธีแก้ไข:** เรียกใช้คำสั่งต่อไปนี้เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่เฉพาะเจาะจง:</span><span class="sxs-lookup"><span data-stu-id="8b06d-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8b06d-112">สิ่งนี้อาจเกิดขึ้นถ้า **RetentionHold** ถูก **เปิดใช้งาน** ในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="8b06d-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8b06d-113">ถ้ามีการวางกล่องจดหมายบน RetentionHold นโยบายการเก็บข้อมูลในกล่องจดหมายจะไม่ถูกประมวลผลในระหว่างช่วงเวลานั้น</span><span class="sxs-lookup"><span data-stu-id="8b06d-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="8b06d-114">สำหรับสนใจเพิ่มเติมเกี่ยวกับการตั้งค่า RetentionHold ให้ดูที่การ[ระงับการเก็บข้อมูลในกล่องจดหมาย](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="8b06d-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8b06d-115">**วิธีแก้ไข**</span><span class="sxs-lookup"><span data-stu-id="8b06d-115">**Solution:**</span></span>
    
  - <span data-ttu-id="8b06d-116">ตรวจสอบสถานะของการตั้งค่า RetentionHold บนกล่องจดหมายที่เฉพาะเจาะจงใน [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="8b06d-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8b06d-117">เรียกใช้คำสั่งต่อไปนี้เพื่อ **ปิดใช้งาน** RetentionHold ในกล่องจดหมายที่เฉพาะเจาะจง:</span><span class="sxs-lookup"><span data-stu-id="8b06d-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8b06d-118">ในตอนนี้ให้เรียกใช้ตัวช่วยสร้างโฟลเดอร์ที่ได้รับการจัดการอีกครั้ง:</span><span class="sxs-lookup"><span data-stu-id="8b06d-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8b06d-119">**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า10เมกะไบต์ผู้ช่วยโฟลเดอร์ที่มีการจัดการจะไม่ประมวลผลกล่องจดหมายโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="8b06d-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8b06d-120">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="8b06d-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="8b06d-121">แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="8b06d-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="8b06d-122">นำนโยบายการเก็บข้อมูลไปใช้กับกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="8b06d-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="8b06d-123">การเพิ่มหรือเอาแท็กการเก็บข้อมูลออก</span><span class="sxs-lookup"><span data-stu-id="8b06d-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="8b06d-124">วิธีระบุชนิดของการเก็บไว้ในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="8b06d-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
