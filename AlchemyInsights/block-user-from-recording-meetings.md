---
title: บล็อกผู้ใช้จากการบันทึกการประชุม
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037066"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="5afa9-102">บล็อกผู้ใช้จากการบันทึกการประชุม</span><span class="sxs-lookup"><span data-stu-id="5afa9-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="5afa9-103">ถ้าคุณต้องการป้องกัน **หรือบล็อกผู้ใช้** บางรายจากการบันทึกการประชุม Teams คุณสามารถบันทึกผ่านการตั้งค่านโยบายการประชุม Teams</span><span class="sxs-lookup"><span data-stu-id="5afa9-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="5afa9-104">ในศูนย์การจัดการ Microsoft Teams ให้ปิดการตั้งค่า **อนุญาตการบันทึก** ระบบคลาวด์ในนโยบายการประชุมที่มอบหมายให้กับผู้ใช้รายนั้น</span><span class="sxs-lookup"><span data-stu-id="5afa9-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="5afa9-105">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="5afa9-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="5afa9-106">เมื่อต้องการตรวจสอบว่าผู้ใช้ที่ระบุได้รับอนุญาตหรือไม่บันทึกการประชุม Teams ให้ใช้การวินิจฉัยการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="5afa9-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="5afa9-107">เรียกใช้คิวรีการสนับสนุนใหม่และพิมพ์ใน **Diag: การบันทึก** การประชุม - การวินิจฉัยจะตรวจสอบการตั้งค่านโยบายของผู้ใช้ที่ระบุและระบุการตั้งค่านโยบาย</span><span class="sxs-lookup"><span data-stu-id="5afa9-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="5afa9-108">โปรดทราบว่าอาจต้องใช้เวลาสองสามชั่วโมงเพื่อให้การตั้งค่านโยบายใหม่มีผล ดังนั้น ถ้าคุณเพิ่งเปลี่ยนแปลง โปรดรอสองสามชั่วโมงก่อนเริ่มการวินิจฉัยอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="5afa9-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="5afa9-109">ดูข้อมูลเพิ่มเติมใน[การเปิดหรือปิดการบันทึกระบบคลาวด์](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="5afa9-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
