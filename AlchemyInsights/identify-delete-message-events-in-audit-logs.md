---
title: ระบุลบเหตุการณ์ข้อความในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716515"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="bf462-102">บันทึกการตรวจสอบสําหรับข้อความอีเมลที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="bf462-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="bf462-103">เริ่มต้นในเดือนมกราคม 2019, Microsoft จะเปิดในกล่องจดหมายตรวจสอบการบันทึกโดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="bf462-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="bf462-104">มิฉะนั้น เมื่อต้องการตรวจสอบลบเหตุการณ์ข้อความสําหรับผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="bf462-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="bf462-105">ถ้าบันทึกการตรวจสอบกล่องจดหมายถูกเปิดใช้งานสําหรับองค์กรของคุณ หรือสําหรับผู้ใช้เฉพาะ ให้ทําตามขั้นตอนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="bf462-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="bf462-106">เข้าสู่ระบบศูนย์[ควบคุม&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="bf462-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="bf462-107">คลิก**ค้นหาและสืบสวน**แล้วเลือก**ค้นหาบันทึกการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="bf462-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="bf462-108">เลือกช่วงวันที่ในฟิลด์**วันที่เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="bf462-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="bf462-109">ระบุชื่อผู้ใช้สําหรับผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ)</span><span class="sxs-lookup"><span data-stu-id="bf462-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="bf462-110">ในฟิลด์**กิจกรรม**ให้เลือก**ข้อความที่ถูกลบจากโฟลเดอร์ รายการที่ถูกลบ**และ**ย้ายข้อความไปยังโฟลเดอร์ รายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="bf462-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="bf462-111">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="bf462-111">Click **Search**.</span></span>

<span data-ttu-id="bf462-112">ในผลลัพธ์ ให้เลือกเรกคอร์ดการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="bf462-112">In the results, select an audit record.</span></span> <span data-ttu-id="bf462-113">ในลอยรายละเอียด ให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="bf462-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="bf462-114">ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ (ตัวอย่างเช่น บรรทัดเรื่องและตําแหน่งที่ตั้งของสินค้าเมื่อถูกลบ) จะแสดงในฟิลด์**Items**</span><span class="sxs-lookup"><span data-stu-id="bf462-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="bf462-115">กระบวนการ**ClientInfoString**คุณสมบัติจะแสดงถ้าการลบที่เกิดขึ้นใน Outlook, Outlook บนเว็บ (เดิมเรียกว่า Outlook Web App), หรืออุปกรณ์อื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="bf462-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="bf462-116">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การกําหนดผู้ติดตั้งการส่งต่ออีเมลสําหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="bf462-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="bf462-117">**หมายเหตุ**: คุณไม่สามารถเรียกรายการที่ถูกลบโดยใช้คุณลักษณะบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="bf462-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="bf462-118">เมื่อต้องการเรียกข้อความที่ถูกลบใน Outlook บนเว็บ ให้ดูที่[กู้คืนรายการที่ถูกลบใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="bf462-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
