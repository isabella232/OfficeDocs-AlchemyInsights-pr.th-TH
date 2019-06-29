---
title: ระบุกิจกรรมกฎของกล่องขาเข้าในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383044"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="cfdba-102">ระบุกิจกรรมกฎของกล่องขาเข้าในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="cfdba-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="cfdba-103">คุณสามารถใช้ค้นหาแฟ้มบันทึกการตรวจสอบใน & ความปลอดภัยศูนย์การปฏิบัติตามกฎระเบียบเพื่อดูเหตุการณ์กฎกล่องขาเข้า (สร้าง แก้ไข และลบกฎกล่องขาเข้า)</span><span class="sxs-lookup"><span data-stu-id="cfdba-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="cfdba-104">เข้าสู่ระบบไปยัง[ศูนย์ปฏิบัติตามกฎระเบียบ & 365 ความปลอดภัยของ Office](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="cfdba-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="cfdba-105">คลิก**ค้นหาและการตรวจสอบ**และ**ค้นหาแฟ้มบันทึกการตรวจสอบบัญชี**ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="cfdba-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="cfdba-106">เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="cfdba-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="cfdba-107">ภายใต้**กิจกรรมในกล่องจดหมาย Exchange**ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเป็น**InboxRule ใหม่สร้าง/ปรับเปลี่ยน/เปิดใช้งาน/ปิดใช้งานกฎของกล่องขาเข้า**</span><span class="sxs-lookup"><span data-stu-id="cfdba-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="cfdba-108">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="cfdba-108">Click **Search**.</span></span>

<span data-ttu-id="cfdba-109">ในผลลัพธ์ เลือกบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="cfdba-109">In the results, select an audit record.</span></span> <span data-ttu-id="cfdba-110">ในเมนูลอยขึ้นรายละเอียด คลิ**กข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="cfdba-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="cfdba-111">ข้อมูลเกี่ยวกับการตั้งค่ากฎกล่องขาเข้าจะแสดงขึ้นในฟิลด์**พารามิเตอร์**</span><span class="sxs-lookup"><span data-stu-id="cfdba-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="cfdba-112">สำหรับข้อมูลเพิ่มเติม ให้ดู[Determining ถ้าผู้ใช้ที่สร้างกฎของกล่องขาเข้า](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="cfdba-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
