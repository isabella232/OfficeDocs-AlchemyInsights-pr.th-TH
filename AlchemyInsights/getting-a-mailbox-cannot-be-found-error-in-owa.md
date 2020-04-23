---
title: 126 การกล่องจดหมายไม่พบข้อผิดพลาดใน OWA หรือไม่
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 72556651c3431379953b05118c688a876eab0632
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720823"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="1fe6a-102">ไม่พบข้อผิดพลาดในกล่องจดหมายใน Outlook บนเว็บใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1fe6a-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="1fe6a-103">ถ้าคุณกําลังใช้ Outlook บนเว็บ และคุณได้รับ**กล่องจดหมายไม่พบข้อผิดพลาด**บัญชีที่คุณใช้ในการเชื่อมต่อกับ Outlook บนเว็บไม่มีสิทธิ์การใช้งาน Exchange Online และดังนั้น ไม่มีกล่องจดหมายที่เกี่ยวข้องกับบัญชี</span><span class="sxs-lookup"><span data-stu-id="1fe6a-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="1fe6a-104">ผู้ดูแลระบบสามารถมอบหมายสิทธิ์การใช้งานให้กับบัญชีของคุณโดยทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="1fe6a-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="1fe6a-105">เปิด[ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/homepage)และไปที่**ผู้ใช้ที่ใช้งานอยู่**ภายใต้ส่วน**ผู้ใช้**และเลือกผู้ใช้ที่เห็นข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="1fe6a-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="1fe6a-106">ในหน้าผู้ใช้ที่เปิดขึ้น ให้ไปที่ส่วน**สิทธิ์การใช้งานและ Apps**เลือกค่า**ตําแหน่งที่ตั้ง**ที่เหมาะสม และกําหนดสิทธิ์การใช้งานที่ประกอบด้วย Exchange Online (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียด)</span><span class="sxs-lookup"><span data-stu-id="1fe6a-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="1fe6a-107">เมื่อเสร็จแล้ว ให้คลิก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="1fe6a-107">When you're finished, click **Save changes**.</span></span>
