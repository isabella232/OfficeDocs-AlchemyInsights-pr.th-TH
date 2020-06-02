---
title: ระบุเหตุการณ์ข้อความลบในบันทึกการตรวจสอบ
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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509007"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="12bed-102">บันทึกการตรวจสอบสําหรับข้อความอีเมลที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="12bed-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="12bed-103">เริ่มต้นในเดือนมกราคม 2019 Microsoft จะเปิดการบันทึกการตรวจสอบกล่องจดหมายตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="12bed-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="12bed-104">มิฉะนั้น คุณต้องเปิดใช้งานการลบกิจกรรมสําหรับการตรวจสอบด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="12bed-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="12bed-105">ถ้ากล่องจดหมายการตรวจสอบการเข้าสู่ระบบถูกเปิดใช้งานแล้ว สําหรับองค์กรของคุณ หรือ สําหรับผู้ใช้เฉพาะ ให้ทําตามขั้นตอนด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="12bed-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="12bed-106">เข้าสู่ระบบศูนย์[ควบคุมการปฏิบัติตามกฎระเบียบ&ความปลอดภัยของ Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="12bed-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="12bed-107">คลิก**ค้นหาและตรวจสอบ**และเลือก**การค้นหาบันทึกการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="12bed-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="12bed-108">เลือกช่วงวันที่ในฟิลด์**วันที่เริ่มต้น**และ**วันที่สิ้นสุด**</span><span class="sxs-lookup"><span data-stu-id="12bed-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="12bed-109">ระบุชื่อผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ)</span><span class="sxs-lookup"><span data-stu-id="12bed-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="12bed-110">ในฟิลด์**กิจกรรม**ให้เลือก**ข้อความที่ถูกลบจากโฟลเดอร์ รายการที่ถูกลบ**และ**ย้ายข้อความไปยังโฟลเดอร์ รายการที่ถูกลบ**</span><span class="sxs-lookup"><span data-stu-id="12bed-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="12bed-111">คลิก**ค้นหา**</span><span class="sxs-lookup"><span data-stu-id="12bed-111">Click **Search**.</span></span>

<span data-ttu-id="12bed-112">ในผลลัพธ์ ให้เลือกเรกคอร์ดการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="12bed-112">In the results, select an audit record.</span></span> <span data-ttu-id="12bed-113">ในรายละเอียด flyout ให้คลิก**ข้อมูลเพิ่มเติม**</span><span class="sxs-lookup"><span data-stu-id="12bed-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="12bed-114">ข้อมูลเพิ่มเติมเกี่ยวกับรายการที่ถูกลบ (ตัวอย่างเช่น บรรทัดเรื่องและตําแหน่งที่ตั้งของสินค้าเมื่อถูกลบ) จะแสดงในฟิลด์**ได้รับผลกระทบItems**</span><span class="sxs-lookup"><span data-stu-id="12bed-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="12bed-115">กระบวนการ**SlyentInfoString**คุณสมบัติจะแสดงถ้าการลบเกิดขึ้นใน Outlook, Outlook บนเว็บ (เดิมเรียกว่า Outlook Web App), หรืออุปกรณ์อื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="12bed-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="12bed-116">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การกําหนดว่าใครเป็นผู้ตั้งค่าการส่งต่ออีเมลสําหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="12bed-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="12bed-117">**หมายเหตุ**: คุณไม่สามารถดึงรายการที่ถูกลบโดยใช้คุณลักษณะบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="12bed-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="12bed-118">เมื่อต้องการเรียกข้อความที่ถูกลบใน Outlook บนเว็บ ให้ดูที่[การกู้คืนรายการที่ถูกลบใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="12bed-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
