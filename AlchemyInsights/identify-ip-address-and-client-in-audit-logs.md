---
title: ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668329"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="9c91e-102">ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="9c91e-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="9c91e-103">ที่อยู่ IP ที่สอดคล้องกับกิจกรรมโดยผู้ใช้ Microsoft ๓๖๕หรือผู้ดูแลระบบจะแสดงอยู่ในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="9c91e-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="9c91e-104">ข้อมูลไคลเอ็นต์ยังถูกบันทึกด้วย</span><span class="sxs-lookup"><span data-stu-id="9c91e-104">The client information is also logged.</span></span> <span data-ttu-id="9c91e-105">ต่อไปนี้เป็นขั้นตอนในการระบุข้อมูลดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="9c91e-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="9c91e-106">ลงชื่อเข้าใช้[ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9c91e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9c91e-107">ไปที่หน้า**Search**  >  **ค้นหาบันทึกการตรวจสอบ**การค้นหา</span><span class="sxs-lookup"><span data-stu-id="9c91e-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="9c91e-108">ถ้าคุณสนใจในกิจกรรมที่เฉพาะเจาะจงให้เลือกกิจกรรมจากรายการ**กิจกรรม**</span><span class="sxs-lookup"><span data-stu-id="9c91e-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="9c91e-109">ถ้าไม่ใช่กิจกรรมทั้งหมดจะถูกส่งกลับสำหรับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="9c91e-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="9c91e-110">**หมายเหตุ**: กิจกรรมบางอย่างอาจไม่พร้อมใช้งานในเมนู **กิจกรรม** อย่างไรก็ตามรายการการตรวจสอบเหล่านั้นจะถูกส่งกลับถ้า **แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมด** ถูกเลือกไว้ (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="9c91e-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="9c91e-111">ระบุชื่อผู้ใช้ในเขตข้อมูล**ผู้ใช้**ให้เลือกช่วงวันที่ที่เหมาะสมสำหรับกิจกรรมแล้วคลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="9c91e-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="9c91e-112">ในผลลัพธ์คุณสามารถดูที่อยู่ IP ของกิจกรรมนั้นในบานหน้าต่างผลลัพธ์ได้</span><span class="sxs-lookup"><span data-stu-id="9c91e-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="9c91e-113">เลือกระเบียนการตรวจสอบเพื่อดูข้อมูลโดยละเอียดในเมนู **รายละเอียดรายละเอียด** (ตัวอย่างเช่นลูกค้าผู้ใช้ที่ดำเนินการการดำเนินการเป็นต้น)</span><span class="sxs-lookup"><span data-stu-id="9c91e-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="9c91e-114">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การค้นหาที่อยู่ IP ของคอมพิวเตอร์ที่ใช้ในการเข้าถึงบัญชีผู้ใช้ที่ถูกบุกรุก](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="9c91e-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
