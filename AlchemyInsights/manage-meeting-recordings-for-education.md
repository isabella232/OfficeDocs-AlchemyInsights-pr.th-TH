---
title: จัดการการบันทึกการประชุมสำหรับการศึกษา
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6131"
- "9002530"
ms.openlocfilehash: 1cc6173c1efcf46081781d5836b71ce19cfa7bc2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695090"
---
# <a name="manage-meeting-recordings-for-education"></a><span data-ttu-id="cb647-102">จัดการการบันทึกการประชุมสำหรับการศึกษา</span><span class="sxs-lookup"><span data-stu-id="cb647-102">Manage meeting recordings for Education</span></span>

<span data-ttu-id="cb647-103">เริ่มต้น  **วันที่20สิงหาคม๒๐๒๐**เมื่อผู้ใช้ที่มีสิทธิ์การใช้งาน a1 (รวมถึง a1 Plus) เริ่มการบันทึกการประชุมของทีมการบันทึกจะพร้อมใช้งานสำหรับ21วัน</span><span class="sxs-lookup"><span data-stu-id="cb647-103">Starting  **August 20, 2020**, when users with A1 (including A1 Plus) licenses start a Teams meeting recording, the recording is available for 21 days.</span></span>

<span data-ttu-id="cb647-104">สำหรับข้อมูลเพิ่มเติมรวมถึงวิธีการบันทึกการประชุมไปยังตำแหน่งที่ตั้งอื่นให้ดูที่[อัปโหลดการบันทึกการประชุมของ Microsoft team ไปยังสตรีม](https://docs.microsoft.com/stream/portal-upload-teams-meeting-recording)</span><span class="sxs-lookup"><span data-stu-id="cb647-104">For more info, including how to save the meeting to another location, see [Upload a Microsoft Teams meeting recording to Stream](https://docs.microsoft.com/stream/portal-upload-teams-meeting-recording).</span></span>

<span data-ttu-id="cb647-105">เราขอแนะนำให้ผู้ดูแลระบบสำหรับองค์กรการศึกษาพิจารณาใช้แพคเกจนโยบายสำหรับความปลอดภัยของนักเรียนและนักการศึกษา</span><span class="sxs-lookup"><span data-stu-id="cb647-105">We recommend that admins for Education organizations consider using policy packages for student and educator safety.</span></span> <span data-ttu-id="cb647-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="cb647-106">For more info, see:</span></span>

- <span data-ttu-id="cb647-107">[แพคเกจนโยบายในทีม Microsoft](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policy-packages-in-microsoft-teams)</span><span class="sxs-lookup"><span data-stu-id="cb647-107">[Policy packages in Microsoft Teams](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policy-packages-in-microsoft-teams).</span></span>  
    
- <span data-ttu-id="cb647-108">[นโยบายที่ควรได้รับมอบหมายสำหรับความปลอดภัยของนักเรียน](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-student-safety)</span><span class="sxs-lookup"><span data-stu-id="cb647-108">[Policies that should be assigned for student safety](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-student-safety).</span></span>

- <span data-ttu-id="cb647-109">[นโยบายที่ควรได้รับมอบหมายให้กับนักการศึกษา](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-educators)</span><span class="sxs-lookup"><span data-stu-id="cb647-109">[Policies that should be assigned for educators](https://docs.microsoft.com/microsoftteams/policy-packages-edu#policies-that-should-be-assigned-for-educators).</span></span>

<span data-ttu-id="cb647-110">ถ้าคุณต้องการจัดการเฉพาะความสามารถในการบันทึกการประชุมให้ดู[เปิดหรือปิดการบันทึกบนคลาวด์](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="cb647-110">If you want to manage only the ability to record meetings, see [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>  

<span data-ttu-id="cb647-111">**หมายเหตุ:** ความสามารถในการบันทึกการประชุมของทีมจะใช้ความพร้อมใช้งานของการส่งกระแสข้อมูลภูมิภาคและประเทศ</span><span class="sxs-lookup"><span data-stu-id="cb647-111">**Note** Teams Meeting Recording capabilities rely on Stream regional and country availability.</span></span> <span data-ttu-id="cb647-112">ถ้าคุณไม่สามารถบันทึกการประชุมได้ให้ดู[ที่ภูมิภาคใดที่ Microsoft Stream โฮสต์ข้อมูลของฉันใน](https://docs.microsoft.com/stream/faq#which-regions-does-microsoft-stream-host-my-data-in)</span><span class="sxs-lookup"><span data-stu-id="cb647-112">If you can't record a meeting, see [Which regions does Microsoft Stream host my data in?](https://docs.microsoft.com/stream/faq#which-regions-does-microsoft-stream-host-my-data-in).</span></span> 

<span data-ttu-id="cb647-113">สำหรับข้อมูลเพิ่มเติมให้ดูที่ฟีเจอร์ที่ได้รับการ[อัปเดต: Microsoft Stream cloud การบันทึกการควบคุมพื้นที่จัดเก็บข้อมูลภูมิภาค](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter?id=MC214327)</span><span class="sxs-lookup"><span data-stu-id="cb647-113">For more information, see [Updated Feature: Microsoft Stream cloud recordings regional storage control](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter?id=MC214327).</span></span>