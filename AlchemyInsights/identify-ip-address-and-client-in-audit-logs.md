---
title: ระบุที่อยู่ IP และไคลเอนต์ในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382972"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="d8a46-102">ระบุที่อยู่ IP และไคลเอนต์ในบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="d8a46-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="d8a46-103">อยู่ IP ที่สอดคล้องกับกิจกรรมโดยผู้ดูแลระบบหรือผู้ใช้ จะปรากฏในบันทึกการตรวจสอบนั้น</span><span class="sxs-lookup"><span data-stu-id="d8a46-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="d8a46-104">ไคลเอ็นต์ข้อมูลยังถูกบันทึกไว้</span><span class="sxs-lookup"><span data-stu-id="d8a46-104">The client information is also logged.</span></span> <span data-ttu-id="d8a46-105">ต่อไปนี้เป็นขั้นตอนเพื่อระบุข้อมูลดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="d8a46-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="d8a46-106">เข้าสู่ระบบไปยัง[ศูนย์ปฏิบัติตามกฎระเบียบ & 365 ความปลอดภัยของ Office](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d8a46-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d8a46-107">คลิก**ค้นหาและการตรวจสอบ**และ**ค้นหาแฟ้มบันทึกการตรวจสอบบัญชี**ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="d8a46-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="d8a46-108">หากคุณสนใจในกิจกรรมหนึ่ง ๆ เลือกค่าจากรายการ**กิจกรรม**</span><span class="sxs-lookup"><span data-stu-id="d8a46-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="d8a46-109">ถ้า ไม่มี กิจกรรมทั้งหมดจะถูกส่งกลับสำหรับผู้ใช้ที่เลือก (การตั้งค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="d8a46-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="d8a46-110">**หมายเหตุ**: กิจกรรมบางอย่างอาจไม่พร้อมใช้งานในเมนู**กิจกรรม** อย่างไรก็ตาม ที่ทำการตรวจสอบสินค้าจะถูกส่งกลับถ้า**แสดงผลลัพธ์สำหรับกิจกรรมทั้งหมดที่**ถูกเลือก (ค่าเริ่มต้น)</span><span class="sxs-lookup"><span data-stu-id="d8a46-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="d8a46-111">ระบุชื่อผู้ใช้ในฟิลด์**ผู้ใช้**เลือกช่วงวันที่เหมาะสมสำหรับกิจกรรม และจากนั้น คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="d8a46-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="d8a46-112">ในผลลัพธ์ คุณสามารถดูอยู่ IP สำหรับกิจกรรมนั้นในบานหน้าต่างผลลัพธ์</span><span class="sxs-lookup"><span data-stu-id="d8a46-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="d8a46-113">เลือกเรกคอร์ดตรวจสอบเพื่อดูข้อมูลรายละเอียดในเมนูลอยขึ้น**รายละเอียด**(ตัวอย่างเช่น ไคลเอ็นต์ ผู้ใช้ที่ทำการดำเนินการ เป็นต้น)</span><span class="sxs-lookup"><span data-stu-id="d8a46-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="d8a46-114">สำหรับข้อมูลเพิ่มเติม ดู[การค้นหาอยู่ IP ของคอมพิวเตอร์ที่ใช้ในการเข้าถึงบัญชีจากการถูกโจมตี](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="d8a46-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
