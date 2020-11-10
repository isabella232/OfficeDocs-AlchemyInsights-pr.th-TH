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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982555"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="eb30d-102">ข้อคิดเห็นเกี่ยวกับรายการ</span><span class="sxs-lookup"><span data-stu-id="eb30d-102">Comments on List items</span></span>

<span data-ttu-id="eb30d-103">ผู้ใช้จะสามารถเพิ่มและลบข้อคิดเห็นในรายการของรายการได้ในเร็วๆนี้</span><span class="sxs-lookup"><span data-stu-id="eb30d-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="eb30d-104">ผู้ใช้สามารถดูข้อคิดเห็นทั้งหมดในตัวเลือกรายการและกรองระหว่างมุมมองที่แสดงข้อคิดเห็นหรือกิจกรรมที่เกี่ยวข้องกับรายการได้</span><span class="sxs-lookup"><span data-stu-id="eb30d-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="eb30d-105">การกำหนด **เวลา** :</span><span class="sxs-lookup"><span data-stu-id="eb30d-105">**Timing** :</span></span>

<span data-ttu-id="eb30d-106">การ **เผยแพร่** ที่กำหนดเป้าหมาย: ค่อยๆย้อนออกในช่วงกลางเดือนตุลาคมและคาดว่าจะเสร็จสิ้นโดยกลางเดือนพฤศจิกายน</span><span class="sxs-lookup"><span data-stu-id="eb30d-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="eb30d-107">การ **เผยแพร่แบบมาตรฐาน** : ค่อยๆย้อนออกในช่วงกลางเดือนพฤศจิกายนและคาดว่าจะเสร็จสิ้นในช่วงต้นเดือนธันวาคม</span><span class="sxs-lookup"><span data-stu-id="eb30d-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="eb30d-108">**ไวร์** : การเผยแพร่ที่กำหนดเป้าหมายสำหรับทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="eb30d-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="eb30d-109">ผู้ใช้จำเป็นต้องบันทึกสิ่งต่อไปนี้ก่อนที่พวกเขาจะสามารถเพิ่มและลบข้อคิดเห็น:</span><span class="sxs-lookup"><span data-stu-id="eb30d-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="eb30d-110">ข้อคิดเห็นให้ทำตามการตั้งค่าสิทธิ์โดยธรรมชาติใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="eb30d-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="eb30d-111">รายการคลาสสิกที่ยังไม่ได้สร้างขึ้นเพื่อแสดงในส่วนติดต่อผู้ใช้ที่ทันสมัยเช่นรายการงานจะไม่มีฟีเจอร์การแสดงข้อคิดเห็นนี้</span><span class="sxs-lookup"><span data-stu-id="eb30d-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="eb30d-112">การแสดงความคิดเห็นเกี่ยวกับรายการในทีมไม่พร้อมใช้งานกับรุ่นนี้</span><span class="sxs-lookup"><span data-stu-id="eb30d-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="eb30d-113">ข้อคิดเห็นไม่ได้รับการทำดัชนีด้วยการค้นหา</span><span class="sxs-lookup"><span data-stu-id="eb30d-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="eb30d-114">ผู้ดูแลระบบสามารถปิดใช้งานฟีเจอร์นี้ได้ที่ระดับองค์กรโดยการเปลี่ยนพารามิเตอร์ **CommentsOnListItemsDisabled** ใน Cmdlet การ **ตั้งค่า-SPOTenant** PowerShell</span><span class="sxs-lookup"><span data-stu-id="eb30d-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="eb30d-115">ในตอนนี้ยังไม่สามารถปิดใช้งานการแสดงข้อคิดเห็นที่ไซต์หรือระดับรายการได้</span><span class="sxs-lookup"><span data-stu-id="eb30d-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="eb30d-116">เราหวังว่าจะมีตัวควบคุมเหล่านี้ในการอัปเดตในภายหลังซึ่งมีแนวโน้มในไตรมาสแรก๒๐๒๑</span><span class="sxs-lookup"><span data-stu-id="eb30d-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
