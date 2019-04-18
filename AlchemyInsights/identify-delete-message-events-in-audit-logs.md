---
title: ระบุเหตุการณ์ข้อความลบในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909621"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="8ddc3-102">บันทึกการตรวจสอบสำหรับข้อความอีเมลที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="8ddc3-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="8ddc3-103">เริ่มต้นในเดือน 2019 มกราคม Microsoft มีการเปิดใช้งานการเข้าสู่ระบบ โดยค่าเริ่มต้นการตรวจสอบกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="8ddc3-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="8ddc3-104">มิฉะนั้น เพื่อทบทวนเหตุการณ์ข้อความลบสำหรับผู้ใช้ที่ระบุ คุณจำเป็นต้องเปิดใช้งานการดำเนินการลบสำหรับการตรวจสอบได้ด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="8ddc3-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="8ddc3-105">ถ้ากล่องจดหมายการตรวจสอบ บันทึกแล้วเปิดใช้งาน สำหรับองค์กรของคุณ หรือผู้ใช้เฉพาะ ให้ทำตามขั้นตอนด้านล่างนี้</span><span class="sxs-lookup"><span data-stu-id="8ddc3-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="8ddc3-106">เข้าสู่ระบบไปยัง[ศูนย์ปฏิบัติตามกฎระเบียบ & 365 ความปลอดภัยของ Office](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="8ddc3-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="8ddc3-107">คลิก**ค้นหาและการตรวจสอบ**และ**ค้นหาแฟ้มบันทึกการตรวจสอบบัญชี**ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="8ddc3-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="8ddc3-108">เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="8ddc3-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="8ddc3-109">ระบุชื่อผู้ใช้สำหรับผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ)</span><span class="sxs-lookup"><span data-stu-id="8ddc3-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="8ddc3-110">ในฟิลด์**กิจกรรม**เลือก**ข้อความที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ**และ**Moved ข้อความไปยังโฟลเดอร์รายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="8ddc3-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="8ddc3-111">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="8ddc3-111">Click **Search**.</span></span>

<span data-ttu-id="8ddc3-112">ในผลลัพธ์ เลือกบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="8ddc3-112">In the results, select an audit record.</span></span> <span data-ttu-id="8ddc3-113">ในเมนูลอยขึ้นรายละเอียด คลิ**กข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="8ddc3-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="8ddc3-114">ข้อมูลเพิ่มเติมเกี่ยวกับรายการถูกลบไปแล้ว (ตัวอย่างเช่น บรรทัดชื่อเรื่องและตำแหน่งที่ตั้งของสินค้าเมื่อถูกลบ) จะแสดงในเขตข้อมูล**AffectedItems**</span><span class="sxs-lookup"><span data-stu-id="8ddc3-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="8ddc3-115">คุณสมบัติ**ClientInfoString**จะแสดงถ้าการลบเกิดขึ้นใน Outlook, Outlook บนเว็บ (ซึ่งเดิมเรียกว่า Outlook Web App), หรืออุปกรณ์อื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="8ddc3-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="8ddc3-116">สำหรับข้อมูลเพิ่มเติม ดู[Determining ที่ติดตั้งอีเมลที่ส่งต่อสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="8ddc3-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="8ddc3-117">**หมายเหตุ**: คุณไม่สามารถเรียกใช้คุณลักษณะแฟ้มบันทึกการตรวจสอบรายการที่ถูกลบได้</span><span class="sxs-lookup"><span data-stu-id="8ddc3-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="8ddc3-118">เมื่อต้องการเรียกข้อความที่ถูกลบใน Outlook บนเว็บ ดู[กู้คืนรายการใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="8ddc3-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
