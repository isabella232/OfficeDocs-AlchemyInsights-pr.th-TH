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
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539192"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="99b3e-102">ระบุกิจกรรมกฎของกล่องขาเข้าในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="99b3e-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="99b3e-103">คุณสามารถใช้ค้นหาแฟ้มบันทึกการตรวจสอบใน & Office 365 Security Center การปฏิบัติตามกฎระเบียบเพื่อดูเหตุการณ์กฎกล่องขาเข้า (สร้าง แก้ไข และลบกฎกล่องขาเข้า)</span><span class="sxs-lookup"><span data-stu-id="99b3e-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="99b3e-104">เข้าสู่ระบบไปยัง[ศูนย์การปฏิบัติตามกฎระเบียบ & ความปลอดภัย 365 Office](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="99b3e-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="99b3e-105">การ**ค้นหา**ไป > เพ**จค้นหาแฟ้มบันทึกการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="99b3e-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="99b3e-106">เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="99b3e-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="99b3e-107">ภายใต้**กิจกรรมในกล่องจดหมาย Exchange**ตรวจสอบฟิลด์**กิจกรรม**ถูกตั้งค่าเป็น**InboxRule ใหม่สร้าง/ปรับเปลี่ยน/เปิดใช้งาน/ปิดใช้งานกฎของกล่องขาเข้า**</span><span class="sxs-lookup"><span data-stu-id="99b3e-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="99b3e-108">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="99b3e-108">Click **Search**.</span></span>

<span data-ttu-id="99b3e-109">ในผลลัพธ์ เลือกบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="99b3e-109">In the results, select an audit record.</span></span> <span data-ttu-id="99b3e-110">ในเมนูลอยขึ้นรายละเอียด คลิ**กข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="99b3e-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="99b3e-111">ข้อมูลเกี่ยวกับการตั้งค่ากฎกล่องขาเข้าจะแสดงขึ้นในฟิลด์**พารามิเตอร์**</span><span class="sxs-lookup"><span data-stu-id="99b3e-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="99b3e-112">สำหรับข้อมูลเพิ่มเติม ให้ดู[Determining ถ้าผู้ใช้ที่สร้างกฎของกล่องขาเข้า](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="99b3e-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
