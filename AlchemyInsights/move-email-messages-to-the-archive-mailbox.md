---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511059"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="4505c-102">ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="4505c-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="4505c-103">ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="4505c-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="4505c-104">ถ้าไม่ใช่ ให้ใช้ขั้นตอน[ในบทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="4505c-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="4505c-105">เมื่อต้องการเก็บถาวรข้อความไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ**Move to archive\*\*\*\*applied automatically to entire mailbox (default) tag**</span><span class="sxs-lookup"><span data-stu-id="4505c-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="4505c-106">ใช้ขั้นตอนในการสร้างแท็ก:[เก็บแท็กเริ่มต้นเก็บถาวร](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)</span><span class="sxs-lookup"><span data-stu-id="4505c-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="4505c-107">จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ลงในนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="4505c-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="4505c-108">ในศูนย์การจัดการ Exchange เลือก**นโยบายการเก็บข้อมูล**>เพิ่ม**แท็กย้ายไปยังเก็บถาวร**นโยบาย>**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="4505c-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="4505c-109">ตอนนี้[กําหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ให้กับกล่องจดหมายของผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="4505c-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="4505c-110">นโยบายเดียวกันจะถูกนําไปใช้กับกล่องจดหมาย**หลัก**และการ**เก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="4505c-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="4505c-111">อาจจําเป็นต้องบังคับโฟลเดอร์ที่มีการจัดการช่วย (MFA) เพื่อเรียกใช้ และใช้การตั้งค่าใหม่ไปยังกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="4505c-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="4505c-112">เรียกใช้คําสั่งต่อไปนี้ในขณะที่เชื่อมต่อกับ[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นผู้ช่วยโฟลเดอร์ที่มีการจัดการสําหรับกล่องจดหมายที่ระบุ:</span><span class="sxs-lookup"><span data-stu-id="4505c-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="4505c-113">เริ่มต้นจัดการFolderAssistant -เอกลักษณ์<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="4505c-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="4505c-114">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ให้ดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสําหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="4505c-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  