---
title: ข้อคิดเห็นเกี่ยวกับรายการ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724173"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="0202d-102">ข้อคิดเห็นเกี่ยวกับรายการ</span><span class="sxs-lookup"><span data-stu-id="0202d-102">Comments on List items</span></span>

<span data-ttu-id="0202d-103">ผู้ใช้สามารถดูข้อคิดเห็นทั้งหมดในตัวเลือกรายการและกรองระหว่างมุมมองที่แสดงข้อคิดเห็นหรือกิจกรรมที่เกี่ยวข้องกับรายการได้</span><span class="sxs-lookup"><span data-stu-id="0202d-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="0202d-104">ผู้ใช้จำเป็นต้องบันทึกสิ่งต่อไปนี้ก่อนที่พวกเขาจะสามารถเพิ่มและลบข้อคิดเห็น:</span><span class="sxs-lookup"><span data-stu-id="0202d-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="0202d-105">ข้อคิดเห็นให้ทำตามการตั้งค่าสิทธิ์โดยธรรมชาติใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="0202d-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="0202d-106">รายการคลาสสิกที่ยังไม่ได้สร้างขึ้นเพื่อแสดงในส่วนติดต่อผู้ใช้ที่ทันสมัยเช่นรายการงานจะไม่มีฟีเจอร์การแสดงข้อคิดเห็นนี้</span><span class="sxs-lookup"><span data-stu-id="0202d-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="0202d-107">การแสดงความคิดเห็นเกี่ยวกับรายการในทีมไม่พร้อมใช้งานกับรุ่นนี้</span><span class="sxs-lookup"><span data-stu-id="0202d-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="0202d-108">ข้อคิดเห็นไม่ได้รับการทำดัชนีด้วยการค้นหา</span><span class="sxs-lookup"><span data-stu-id="0202d-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="0202d-109">ผู้ดูแลระบบสามารถปิดใช้งานฟีเจอร์นี้ได้ที่ระดับองค์กรโดยการเปลี่ยนพารามิเตอร์ **CommentsOnListItemsDisabled** ใน Cmdlet การ **ตั้งค่า-SPOTenant** PowerShell</span><span class="sxs-lookup"><span data-stu-id="0202d-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="0202d-110">ในตอนนี้ยังไม่สามารถปิดใช้งานการแสดงข้อคิดเห็นที่ไซต์หรือระดับรายการได้</span><span class="sxs-lookup"><span data-stu-id="0202d-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="0202d-111">เราหวังว่าจะมีตัวควบคุมเหล่านี้ในการอัปเดตในภายหลังซึ่งมีแนวโน้มในไตรมาสแรก๒๐๒๑</span><span class="sxs-lookup"><span data-stu-id="0202d-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
