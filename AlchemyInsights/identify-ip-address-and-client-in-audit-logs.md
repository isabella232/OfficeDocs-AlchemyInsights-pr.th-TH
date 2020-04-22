---
title: ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716407"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ab697-102">ระบุที่อยู่ IP และไคลเอ็นต์ในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="ab697-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ab697-103">อยู่ IP ที่สอดคล้องกับกิจกรรม โดยผู้ใช้ Microsoft 365 หรือผู้ดูแลระบบจะแสดงในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="ab697-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ab697-104">ข้อมูลไคลเอ็นต์จะถูกบันทึกด้วย</span><span class="sxs-lookup"><span data-stu-id="ab697-104">The client information is also logged.</span></span> <span data-ttu-id="ab697-105">ต่อไปนี้เป็นขั้นตอนในการระบุข้อมูลดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="ab697-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ab697-106">เข้าสู่ระบบศูนย์[การปฏิบัติตาม&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="ab697-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ab697-107">ไปที่หน้า**ค้นหาบันทึกการตรวจสอบ\*\*\*\*การค้นหา** > </span><span class="sxs-lookup"><span data-stu-id="ab697-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ab697-108">ถ้าคุณสนใจกิจกรรมเฉพาะ ให้เลือกกิจกรรมจากรายการ**กิจกรรม**</span><span class="sxs-lookup"><span data-stu-id="ab697-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ab697-109">ถ้าไม่ กิจกรรมทั้งหมดจะถูกส่งกลับสําหรับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="ab697-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ab697-110">**หมายเหตุ**: กิจกรรมบางอย่างอาจไม่มีในเมนู**กิจกรรม** อย่างไรก็ตาม รายการการตรวจสอบเหล่านั้นจะถูกส่งกลับถ้า**แสดงผลลัพธ์สําหรับกิจกรรมทั้งหมด**ถูกเลือกไว้ (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="ab697-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ab697-111">ระบุชื่อผู้ใช้ในฟิลด์**ผู้ใช้**ให้เลือกช่วงวันที่ที่เหมาะสมสําหรับกิจกรรม แล้วคลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="ab697-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ab697-112">ในผลลัพธ์ คุณจะเห็นที่อยู่ IP สําหรับกิจกรรมนั้นในบานหน้าต่างผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="ab697-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ab697-113">เลือกเรกคอร์ดการตรวจสอบเพื่อดูข้อมูลโดยละเอียด**ในรายละเอียดลอย**(ตัวอย่างเช่น ลูกค้า ผู้ใช้ที่ดําเนินการ กระทํา ฯลฯ)</span><span class="sxs-lookup"><span data-stu-id="ab697-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ab697-114">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การค้นหาที่อยู่ IP ของคอมพิวเตอร์ที่ใช้ในการเข้าถึงบัญชีที่ถูกบุกรุก](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="ab697-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
