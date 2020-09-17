---
title: ระบุกิจกรรมกฎสำหรับกล่องจดหมายเข้าในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779070"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="1f69f-102">ระบุกิจกรรมกฎสำหรับกล่องจดหมายเข้าในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="1f69f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="1f69f-103">คุณสามารถใช้การค้นหาบันทึกการตรวจสอบในศูนย์การรักษาความปลอดภัย & ของ Microsoft ๓๖๕เพื่อดูเหตุการณ์ของกฎสำหรับกล่องจดหมายเข้า (การสร้างการปรับเปลี่ยนและการลบกฎของกล่องจดหมายเข้า)</span><span class="sxs-lookup"><span data-stu-id="1f69f-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="1f69f-104">ลงชื่อเข้าใช้[ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1f69f-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1f69f-105">ไปที่หน้า**Search**  >  **ค้นหาบันทึกการตรวจสอบ**การค้นหา</span><span class="sxs-lookup"><span data-stu-id="1f69f-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="1f69f-106">เลือกช่วงวันที่ในเขตข้อมูลวันที่**เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="1f69f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="1f69f-107">ภายใต้**กิจกรรมกล่องจดหมาย Exchange**ให้ตรวจสอบว่าเขตข้อมูล**กิจกรรม**ถูกตั้งค่าเป็น**InboxRule สร้าง/แก้ไข/เปิดใช้งานกฎกล่องจดหมายเข้าใหม่**</span><span class="sxs-lookup"><span data-stu-id="1f69f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="1f69f-108">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="1f69f-108">Click **Search**.</span></span>

<span data-ttu-id="1f69f-109">ในผลลัพธ์ให้เลือกระเบียนการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="1f69f-109">In the results, select an audit record.</span></span> <span data-ttu-id="1f69f-110">ในเมนูรายละเอียดให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="1f69f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1f69f-111">ข้อมูลเกี่ยวกับการตั้งค่ากฎสำหรับกล่องจดหมายเข้าจะแสดงอยู่ในเขตข้อมูล**พารามิเตอร์**</span><span class="sxs-lookup"><span data-stu-id="1f69f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="1f69f-112">สำหรับข้อมูลเพิ่มเติมให้ดูที่[การกำหนดว่าผู้ใช้สร้างกฎกล่องจดหมายเข้าหรือ](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)ไม่</span><span class="sxs-lookup"><span data-stu-id="1f69f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
