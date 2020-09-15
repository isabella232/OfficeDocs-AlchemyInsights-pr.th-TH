---
title: ๑๒๖การรับกล่องจดหมายไม่พบข้อผิดพลาดใน OWA ใช่หรือไม่
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706769"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="776c1-102">การรับกล่องจดหมายไม่พบข้อผิดพลาดใน Outlook บนเว็บ</span><span class="sxs-lookup"><span data-stu-id="776c1-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="776c1-103">ถ้าคุณกำลังใช้ Outlook บนเว็บและคุณได้รับ **กล่องจดหมายไม่พบ** ข้อผิดพลาดบัญชีผู้ใช้ที่คุณใช้ในการเชื่อมต่อกับ Outlook บนเว็บไม่มีสิทธิ์การใช้งาน Exchange Online ดังนั้นจึงไม่มีกล่องจดหมายที่เชื่อมโยงกับบัญชีผู้ใช้นั้น</span><span class="sxs-lookup"><span data-stu-id="776c1-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="776c1-104">ผู้ดูแลระบบของคุณสามารถกำหนดสิทธิ์การใช้งานให้กับบัญชีผู้ใช้ของคุณได้โดยทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="776c1-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="776c1-105">เปิด [ศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/homepage) แล้วไปที่ **ผู้ใช้ที่ใช้งานอยู่** ภายใต้ส่วน **ผู้ใช้** แล้วเลือกผู้ใช้ที่เห็นข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="776c1-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="776c1-106">ในหน้าผู้ใช้ที่เปิดขึ้นให้ไปที่ส่วนสิทธิ์การใช้งาน **และแอป** เลือกค่า **ตำแหน่งที่ตั้ง** ที่เหมาะสมและกำหนดสิทธิ์การใช้งานที่มี Exchange Online (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียด)</span><span class="sxs-lookup"><span data-stu-id="776c1-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="776c1-107">เมื่อคุณดำเนินการเสร็จสิ้นแล้วให้คลิก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="776c1-107">When you're finished, click **Save changes**.</span></span>
