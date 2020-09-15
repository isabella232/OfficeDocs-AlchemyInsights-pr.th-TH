---
title: ระบุการลบเหตุการณ์ข้อความในบันทึกการตรวจสอบ
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696532"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="e0ba0-102">บันทึกการตรวจสอบสำหรับข้อความอีเมลที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="e0ba0-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="e0ba0-103">เริ่มต้นในเดือนมกราคม๒๐๑๙ Microsoft จะเปิดใช้งานการบันทึกการตรวจสอบของกล่องจดหมายตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="e0ba0-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="e0ba0-104">มิฉะนั้นถ้าต้องการรีวิวลบเหตุการณ์ข้อความสำหรับผู้ใช้ที่เฉพาะเจาะจงคุณจำเป็นต้องเปิดใช้งานการดำเนินการลบสำหรับการตรวจสอบด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="e0ba0-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="e0ba0-105">ถ้ามีการเปิดใช้งานการบันทึกการตรวจสอบของกล่องจดหมายสำหรับองค์กรของคุณหรือสำหรับผู้ใช้ที่ระบุไว้แล้วให้ทำตามขั้นตอนด้านล่างนี้</span><span class="sxs-lookup"><span data-stu-id="e0ba0-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="e0ba0-106">ลงชื่อเข้าใช้ใน [ศูนย์การรักษาความปลอดภัย Microsoft ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e0ba0-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e0ba0-107">คลิก**ค้นหาและ\*\*\*\*ตรวจสอบแล้วเลือกค้นหาบันทึกการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e0ba0-108">เลือกช่วงวันที่ในเขตข้อมูลวันที่**เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e0ba0-109">ระบุชื่อผู้ใช้สำหรับผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ)</span><span class="sxs-lookup"><span data-stu-id="e0ba0-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="e0ba0-110">ในเขตข้อมูล**กิจกรรม**ให้เลือก**ข้อความที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ**และ**ย้ายข้อความไปยังโฟลเดอร์รายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="e0ba0-111">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-111">Click **Search**.</span></span>

<span data-ttu-id="e0ba0-112">ในผลลัพธ์ให้เลือกระเบียนการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="e0ba0-112">In the results, select an audit record.</span></span> <span data-ttu-id="e0ba0-113">ในเมนูรายละเอียดให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e0ba0-114">ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ (ตัวอย่างเช่นบรรทัดชื่อเรื่องและตำแหน่งที่ตั้งของรายการเมื่อถูกลบ) จะแสดงอยู่ในเขตข้อมูล**AffectedItems**</span><span class="sxs-lookup"><span data-stu-id="e0ba0-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="e0ba0-115">คุณสมบัติ **ClientInfoString** จะแสดงถ้าการลบเกิดขึ้นใน Outlook, outlook บนเว็บ (เดิมเรียกว่า Outlook web App) หรืออุปกรณ์อื่นๆ</span><span class="sxs-lookup"><span data-stu-id="e0ba0-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="e0ba0-116">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การกำหนดผู้ที่ตั้งค่าการส่งต่ออีเมลสำหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="e0ba0-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="e0ba0-117">**หมายเหตุ**: คุณไม่สามารถเรียกคืนรายการที่ถูกลบโดยใช้ฟีเจอร์บันทึกการตรวจสอบได้</span><span class="sxs-lookup"><span data-stu-id="e0ba0-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="e0ba0-118">เมื่อต้องการเรียกคืนข้อความที่ถูกลบใน Outlook บนเว็บให้ดู[กู้คืนรายการที่ถูกลบใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="e0ba0-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
