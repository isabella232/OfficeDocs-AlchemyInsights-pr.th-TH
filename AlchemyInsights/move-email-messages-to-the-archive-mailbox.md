---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวร
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713665"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="9a0d2-102">ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="9a0d2-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="9a0d2-103">ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="9a0d2-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="9a0d2-104">ถ้าไม่ ใช้ขั้นตอน[ในบทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร</span><span class="sxs-lookup"><span data-stu-id="9a0d2-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="9a0d2-105">หากต้องการเก็บถาวรข้อความโดยอัตโนมัติไปยังกล่องจดหมายเก็บถาวร**Move to archive\*\*\*\*applied automatically to entire mailbox (default) tag**</span><span class="sxs-lookup"><span data-stu-id="9a0d2-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="9a0d2-106">ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กเริ่มต้นเก็บถาวร](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)</span><span class="sxs-lookup"><span data-stu-id="9a0d2-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="9a0d2-107">จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ในนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="9a0d2-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="9a0d2-108">ในศูนย์การจัดการ Exchange ให้เลือก**นโยบายการเก็บข้อมูล**>เพิ่ม **>\*\*\*\*แท็ก**</span><span class="sxs-lookup"><span data-stu-id="9a0d2-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="9a0d2-109">ตอนนี้[กําหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ไปยังกล่องจดหมายของผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="9a0d2-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="9a0d2-110">นโยบายเดียวกันจะนําไปใช้กับทั้ง**หลัก**และกล่องจดหมาย**การเก็บถาวร**</span><span class="sxs-lookup"><span data-stu-id="9a0d2-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="9a0d2-111">คุณอาจจําเป็นต้องบังคับให้มีการจัดการโฟลเดอร์ผู้ช่วย (MFA) เพื่อเรียกใช้ และใช้การตั้งค่าใหม่ไปยังกล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="9a0d2-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="9a0d2-112">เรียกใช้คําสั่งต่อไปนี้ขณะเชื่อมต่อกับ[PowerShell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นตัวจัดการโฟลเดอร์ช่วยสําหรับกล่องจดหมายที่ระบุ:</span><span class="sxs-lookup"><span data-stu-id="9a0d2-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="9a0d2-113">เริ่มต้นจัดการโฟลเดอร์ผู้ช่วย -ข้อมูลเฉพาะตัว<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="9a0d2-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="9a0d2-114">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ให้ดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสําหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="9a0d2-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  