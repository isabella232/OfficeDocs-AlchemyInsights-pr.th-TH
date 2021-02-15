---
title: บล็อกลายเซ็นอีเมลที่ผู้ใช้สร้างขึ้น
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243637"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="4ecb3-102">บล็อกลายเซ็นอีเมลที่ผู้ใช้สร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="4ecb3-102">Block user-made email signatures</span></span>

<span data-ttu-id="4ecb3-103">วิธีแก้ไขต่อไปนี้ใช้ได้กับลายเซ็นอีเมลที่สร้างใน Outlook บนเว็บเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="4ecb3-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="4ecb3-104">คุณสามารถบล็อกลายเซ็นในแอป Outlook ได้ถ้าคุณมี Exchange Server ภายในองค์กรเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="4ecb3-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="4ecb3-105">ในศูนย์การจัดการ ให้เลือก **ศูนย์การจัดการ**  >  **Exchange**</span><span class="sxs-lookup"><span data-stu-id="4ecb3-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="4ecb3-106">คลิก **สิทธิ์**  >  **นโยบาย Outlook Web App**</span><span class="sxs-lookup"><span data-stu-id="4ecb3-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="4ecb3-107">เลือกนโยบาย แล้วคลิกไอคอนรูปดินสอเพื่อแก้ไข</span><span class="sxs-lookup"><span data-stu-id="4ecb3-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="4ecb3-108">คลิก  >  **ตัวเลือกฟีเจอร์** เพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="4ecb3-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="4ecb3-109">ภายใต้ **ประสบการณ์** การใช้งานของผู้ใช้ **ให้ล้างกล่องกา** เครื่องหมาย ลายเซ็นอีเมล **แล้วคลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="4ecb3-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="4ecb3-110">**สําคัญ:** ถ้าลายเซ็นถูกเพิ่มก่อนที่จะล้างกล่องกาเครื่องหมายนี้ ผู้ใช้จะยังคงสามารถใช้ลายเซ็นได้</span><span class="sxs-lookup"><span data-stu-id="4ecb3-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="4ecb3-111">ขอให้พวกเขาลบออก</span><span class="sxs-lookup"><span data-stu-id="4ecb3-111">Ask them to remove it.</span></span>
