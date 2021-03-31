---
title: 126 ไม่พบข้อผิดพลาดการรับกล่องจดหมายใน OWA
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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426681"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="1ba4c-102">พบข้อผิดพลาดไม่พบกล่องจดหมายใน Outlook บนเว็บใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1ba4c-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="1ba4c-103">ถ้าคุณใช้ Outlook บนเว็บ และไม่พบกล่องจดหมายจากข้อผิดพลาด บัญชีที่คุณใช้ในการเชื่อมต่อกับ Outlook บนเว็บจึงไม่มีสิทธิ์การใช้งาน Exchange Online ดังนั้นจึงไม่มีกล่องจดหมายที่เชื่อมโยงกับบัญชี</span><span class="sxs-lookup"><span data-stu-id="1ba4c-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="1ba4c-104">ผู้ดูแลระบบของคุณสามารถกําหนดสิทธิการใช้งานให้กับบัญชีของคุณโดยปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="1ba4c-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="1ba4c-105">เปิด [ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/homepage)และ **ไปที่** ผู้ใช้ที่ใช้งานอยู่ภายใต้ส่วน ผู้ใช้ แล้วเลือกผู้ใช้ที่เห็นข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="1ba4c-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="1ba4c-106">ในหน้าผู้ใช้ที่เปิดขึ้น ให้ไปที่ส่วน สิทธิ์การใช้งานและ **แอป** เลือกค่าสถานที่ที่เหมาะสม และกําหนดสิทธิ์การใช้งานที่มี Exchange Online (ขยายสิทธิ์การใช้งานเพื่อดูรายละเอียด)</span><span class="sxs-lookup"><span data-stu-id="1ba4c-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="1ba4c-107">เมื่อคุณเสร็จสิ้น ให้คลิก **บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="1ba4c-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="1ba4c-108">ในบางกรณี ถ้าสิทธิ์การใช้งานถูกมอบหมายให้กับบัญชีผู้ใช้อยู่แล้ว การเอาออกและการมอบหมายสิทธิ์การใช้งานใหม่จะช่วยแก้ไขปัญหาและเตรียมใช้งานได้อย่างถูกต้องในระบบ ดังนี้</span><span class="sxs-lookup"><span data-stu-id="1ba4c-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="1ba4c-109">ตรวจสอบเพื่อดูว่าการสมัครใช้งาน M365 Exchange Online (และอื่นๆ ถ้าคุณมี) เป็นการสมัครใช้งานปัจจุบันและยังไม่หมดอายุเมื่อเร็วๆ นี้</span><span class="sxs-lookup"><span data-stu-id="1ba4c-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="1ba4c-110">เมื่อคุณตรวจสอบให้แน่ใจว่าการสมัครใช้งานของคุณยังไม่หมดอายุและมีการมอบหมายสิทธิ์การใช้งานที่ถูกต้องให้กับบัญชีผู้ใช้ อาจใช้เวลาถึง 24 ชั่วโมงในการเตรียมสิทธิ์การใช้งาน ดังนั้นคุณอาจต้องรอให้ปัญหาของคุณแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="1ba4c-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="1ba4c-111">ดูข้อมูลเพิ่มเติมได้ที่ [กําหนดและจัดการ](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="1ba4c-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>