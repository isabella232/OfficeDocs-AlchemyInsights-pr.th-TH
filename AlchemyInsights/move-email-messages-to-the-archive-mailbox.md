---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวร
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799799"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="46eb1-102">ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="46eb1-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="46eb1-103">ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนสุดของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหาในการย้ายอีเมลไปยังกล่องจดหมายเก็บถาวรของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="46eb1-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="46eb1-104">ยืนยันว่า **กล่องจดหมายเก็บถาวร** ถูกเปิดใช้งานแล้ว</span><span class="sxs-lookup"><span data-stu-id="46eb1-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="46eb1-105">ถ้าไม่ใช่ให้ใช้ขั้นตอนใน [บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="46eb1-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="46eb1-106">เมื่อต้องการเก็บถาวรข้อความโดยอัตโนมัติไปยังกล่องจดหมายเก็บถาวรแท็กการเก็บข้อมูลที่มีการดำเนินการ**ย้ายไปยังการเก็บถาวร**ต้องถูกตั้งค่าให้**นำไปใช้โดยอัตโนมัติไปยังแท็กกล่องจดหมาย (ค่าเริ่มต้น) ทั้งหมด**</span><span class="sxs-lookup"><span data-stu-id="46eb1-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="46eb1-107">ใช้ขั้นตอนต่อไปนี้เพื่อสร้างแท็ก:[แท็กเริ่มต้นของการเก็บถาวร](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)</span><span class="sxs-lookup"><span data-stu-id="46eb1-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="46eb1-108">ถัดไปให้เพิ่มแท็ก **เก็บถาวร** ลงในนโยบายการเก็บข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="46eb1-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="46eb1-109">ในศูนย์การจัดการ Exchange ให้เลือก**นโยบายการเก็บข้อมูล**> เพิ่ม**แท็กย้ายไปยังการเก็บถาวร**ในนโยบาย >**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="46eb1-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="46eb1-110">ในตอนนี้ให้ [กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ให้กับกล่องจดหมายของผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="46eb1-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="46eb1-111">นโยบายเดียวกันจะถูกนำไปใช้กับทั้งกล่องจดหมาย**หลัก**และกล่องจดหมาย**เก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="46eb1-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="46eb1-112">คุณอาจจำเป็นต้องบังคับใช้ตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการ (MFA) เพื่อเรียกใช้และนำการตั้งค่าใหม่ไปใช้กับกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="46eb1-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="46eb1-113">เรียกใช้คำสั่งต่อไปนี้ในขณะ [ที่เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่เฉพาะเจาะจง:</span><span class="sxs-lookup"><span data-stu-id="46eb1-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="46eb1-114">เริ่มต้น-ManagedFolderAssistant-ข้อมูลประจำตัว <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="46eb1-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="46eb1-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวรให้ดู[ที่ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="46eb1-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  