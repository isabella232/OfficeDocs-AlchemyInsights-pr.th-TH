---
title: ย้ายข้อความทาง e-mail ไปยังกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822181"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="69657-102">ย้ายเมลไปยังกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="69657-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="69657-103">ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="69657-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="69657-104">ถ้าไม่ให้ใช้ขั้นตอนใน[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="69657-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="69657-105">ในการเก็บถาวรข้อความไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติจะต้องตั้งค่าแท็กการเก็บข้อมูลที่มีการ**ย้ายไปยังการเก็บถาวร**การดำเนินการที่จะ**นำไปใช้โดยอัตโนมัติไปยังกล่องจดหมายทั้งหมด (เริ่มต้น)**</span><span class="sxs-lookup"><span data-stu-id="69657-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="69657-106">ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กเริ่มต้นที่เก็บถาวร](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)</span><span class="sxs-lookup"><span data-stu-id="69657-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="69657-107">จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ในนโยบายการเก็บข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="69657-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="69657-108">ในศูนย์ดูแล Exchange เลือกนโยบายการ**เก็บข้อมูล**> เพิ่มการ**ย้ายไปยังแท็กเก็บถาวร**ไปยังนโยบาย >**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="69657-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="69657-109">ตอนนี้[กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ให้กับกล่องจดหมายของผู้ใช้ที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="69657-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="69657-110">นโยบายเดียวกันจะถูกนำไปใช้กับทั้งกล่องจดหมาย**หลัก**และ**เก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="69657-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="69657-111">คุณอาจจำเป็นต้องบังคับให้มีการจัดการโฟลเดอร์ผู้ช่วย (MFA) เพื่อเรียกใช้และใช้การตั้งค่าใหม่กับกล่องจดหมายของตัวเอง</span><span class="sxs-lookup"><span data-stu-id="69657-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="69657-112">เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นผู้ช่วยโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่ระบุ:</span><span class="sxs-lookup"><span data-stu-id="69657-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="69657-113">ผู้ช่วยเริ่มต้นการจัดการ-เอกลักษณ์<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="69657-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="69657-114">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวรโปรดดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="69657-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  