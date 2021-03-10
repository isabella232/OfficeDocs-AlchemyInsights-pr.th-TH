---
title: ตัวอย่าง Microsoft Defender ของนโยบายสิ่งที่แนบมาที่ปลอดภัยของ Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695188"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="aaa37-102">ตัวอย่าง Microsoft Defender ของนโยบายสิ่งที่แนบมาที่ปลอดภัยของ Office 365</span><span class="sxs-lookup"><span data-stu-id="aaa37-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="aaa37-103">การตั้งค่าเหล่านี้จะเปิดใช้งานนโยบายที่เรียกว่า *ไม่มีความล่าช้า* ที่ส่งข้อความทันที แล้วแนบสิ่งที่แนบมาใหม่หลังจากสแกน:</span><span class="sxs-lookup"><span data-stu-id="aaa37-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="aaa37-104">**ชื่อ**: ไม่มีความล่าช้า</span><span class="sxs-lookup"><span data-stu-id="aaa37-104">**Name**: No delays</span></span>
- <span data-ttu-id="aaa37-105">**รายละเอียด**: ส่งข้อความทันทีและแนบไฟล์แนบใหม่หลังจากสแกน</span><span class="sxs-lookup"><span data-stu-id="aaa37-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="aaa37-106">**ตอบกลับ**: **เลือกตัวเลือกการส่ง** แบบไดนามิก</span><span class="sxs-lookup"><span data-stu-id="aaa37-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="aaa37-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="aaa37-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="aaa37-108">**เปลี่ยนเส้นทางส่วน** สิ่งที่แนบมา: **เลือกตัวเลือกเพื่อเปิดใช้งาน** การเปลี่ยนเส้นทาง แล้วใส่ที่อยู่อีเมลของผู้ดูแลระบบส่วนกลาง Microsoft 365 ผู้ดูแลระบบความปลอดภัย หรือนักวิเคราะห์ความปลอดภัยที่จะตรวจสอบสิ่งที่แนบมาที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="aaa37-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="aaa37-109">**ส่วน ใช้กับ** : **เลือกโดเมนผู้รับ** แล้วเลือกโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="aaa37-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="aaa37-110">**เลือก** เพิ่ม **แล้วเลือก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="aaa37-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="aaa37-111">เมื่อเสร็จแล้ว ให้เลือก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="aaa37-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="aaa37-112">เมื่อต้องการเรียนรู้เพิ่มเติม ดู[สิ่งที่แนบมาที่ปลอดภัยใน Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="aaa37-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
