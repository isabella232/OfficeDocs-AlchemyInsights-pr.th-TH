---
title: ปิดใช้งานการแชท
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6889"
- "9000738"
ms.openlocfilehash: b6041dd41d0d94b832b962518c73560737684ce1
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089160"
---
# <a name="disable-chat"></a><span data-ttu-id="f0cb0-102">ปิดใช้งานการแชท</span><span class="sxs-lookup"><span data-stu-id="f0cb0-102">Disable chat</span></span>

<span data-ttu-id="f0cb0-103">เมื่อต้องการปิดใช้งานการแชทสำหรับองค์กรของคุณคุณสามารถสร้างนโยบายที่จะช่วยให้คุณสามารถควบคุมฟีเจอร์การแชทและการรับส่งข้อความแชนแนลที่พร้อมใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="f0cb0-103">To disable chat for your organization, you can create policies that will allow you to control which chat and channel messaging features are available.</span></span> <span data-ttu-id="f0cb0-104">มีหลายวิธีในการทำเช่นนี้ขึ้นอยู่กับวิธีที่คุณต้องการกำหนดค่าการแชท</span><span class="sxs-lookup"><span data-stu-id="f0cb0-104">There are several ways to accomplish this, depending on how you need to configure chat.</span></span>

- <span data-ttu-id="f0cb0-105">การ **ส่งข้อ** ความ: ในศูนย์การจัดการทีมให้ไปที่ [นโยบายการส่งข้อ](https://admin.teams.microsoft.com/)ความแล้วสลับเปิดหรือ **ปิด** การ **แชท**</span><span class="sxs-lookup"><span data-stu-id="f0cb0-105">**Messaging**: In the Teams admin center,  go to [Messaging policies](https://admin.teams.microsoft.com/), and toggle **Chat On** or **Off**.</span></span> <span data-ttu-id="f0cb0-106">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการส่งข้อความแบบกำหนดเองและวิธีการกำหนดนโยบายให้กับผู้ใช้ให้ดู[ที่จัดการนโยบายการส่งข้อความในทีม](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="f0cb0-106">For more information on custom messaging policies and how to assign policies to users, see [Manage messaging policies in Teams](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams).</span></span>
- <span data-ttu-id="f0cb0-107">การ **ประชุม**: ในศูนย์การจัดการทีมให้ไปที่ [นโยบายการประชุม](https://admin.teams.microsoft.com/)-การตั้งค่าสำหรับการแชทจะอนุญาตให้มีการ **แชทในการประชุม**</span><span class="sxs-lookup"><span data-stu-id="f0cb0-107">**Meeting**: In the Teams admin center, go to [Meeting policies](https://admin.teams.microsoft.com/) - The setting for chat is **Allow chat in meetings**.</span></span> <span data-ttu-id="f0cb0-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสร้างนโยบายการประชุมแบบกำหนดเองให้ดู[ที่จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)และ[อนุญาตการสนทนาในการประชุม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-chat-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="f0cb0-108">For more information on creating custom meeting policies, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) and [Allow chat in meetings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-chat-in-meetings).</span></span>
- <span data-ttu-id="f0cb0-109">**ผู้ใช้ที่เป็นผู้เยี่ยมชม**: คุณสามารถกำหนดค่านโยบายการเข้าถึงของผู้เยี่ยมชมเพื่ออนุญาตให้ผู้ใช้สามารถเข้าถึงการแชทได้ที่สามารถสลับเปิดหรือ **ปิด** การ **แชท**</span><span class="sxs-lookup"><span data-stu-id="f0cb0-109">**Guest Users**: You can configure guest access policies to allow guests to have access to the chat, who can toggle **Chat On** or **Off**.</span></span> <span data-ttu-id="f0cb0-110">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[กำหนดค่าการเข้าถึงของผู้เยี่ยมชมในศูนย์การจัดการทีม](https://docs.microsoft.com/microsoftteams/set-up-guests#configure-guest-access-in-the-teams-admin-center)</span><span class="sxs-lookup"><span data-stu-id="f0cb0-110">For more information, please refer to [Configure guest access in the Teams admin center](https://docs.microsoft.com/microsoftteams/set-up-guests#configure-guest-access-in-the-teams-admin-center).</span></span>
- <span data-ttu-id="f0cb0-111">**นักเรียน**: เมื่อต้องการปิดใช้งานการแชทสำหรับนักเรียนให้ดูตัวเลือกสำหรับการอนุญาตการแชทในการประชุมและการอนุญาตให้มีการสนทนา1:1 ใน [นโยบายทีมและแพคเกจนโยบายสำหรับการศึกษา](https://docs.microsoft.com/microsoftteams/policy-packages-edu)</span><span class="sxs-lookup"><span data-stu-id="f0cb0-111">**Students**: To disable chat for a student, see the options for allowing chat in meetings and for allowing a 1:1 chat in [Teams policies and policy packages for Education](https://docs.microsoft.com/microsoftteams/policy-packages-edu).</span></span>





