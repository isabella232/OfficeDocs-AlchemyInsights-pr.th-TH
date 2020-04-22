---
title: ระบุกิจกรรมกฎกล่องจดหมายเข้าในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716443"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="b4c7a-102">ระบุกิจกรรมกฎกล่องจดหมายเข้าในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="b4c7a-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="b4c7a-103">คุณสามารถใช้การค้นหาบันทึกการตรวจสอบใน Microsoft 365 Security & ศูนย์การปฏิบัติตามกฎระเบียบเพื่อดูเหตุการณ์กฎกล่องขาเข้า (การสร้าง ปรับเปลี่ยน และการลบกฎของกล่องขาเข้า)</span><span class="sxs-lookup"><span data-stu-id="b4c7a-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="b4c7a-104">เข้าสู่ระบบศูนย์[การปฏิบัติตาม&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b4c7a-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="b4c7a-105">ไปที่หน้า**ค้นหาบันทึกการตรวจสอบ\*\*\*\*การค้นหา** > </span><span class="sxs-lookup"><span data-stu-id="b4c7a-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="b4c7a-106">เลือกช่วงวันที่ในฟิลด์**วันที่เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="b4c7a-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="b4c7a-107">ภายใต้**กิจกรรมกล่องจดหมาย Exchange**ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเป็น**สร้าง/ปรับเปลี่ยน/เปิด/ปิด/กฎของกล่องขาเข้า**</span><span class="sxs-lookup"><span data-stu-id="b4c7a-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="b4c7a-108">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="b4c7a-108">Click **Search**.</span></span>

<span data-ttu-id="b4c7a-109">ในผลลัพธ์ ให้เลือกเรกคอร์ดการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="b4c7a-109">In the results, select an audit record.</span></span> <span data-ttu-id="b4c7a-110">ในลอยรายละเอียด ให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="b4c7a-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b4c7a-111">ข้อมูลเกี่ยวกับการตั้งค่ากฎกล่องจดหมายเข้าจะแสดงอยู่ในฟิลด์**พารามิเตอร์**</span><span class="sxs-lookup"><span data-stu-id="b4c7a-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="b4c7a-112">สําหรับข้อมูลเพิ่มเติม โปรดดู[การกําหนดถ้าผู้ใช้สร้างกฎของกล่องขาเข้า](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="b4c7a-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
