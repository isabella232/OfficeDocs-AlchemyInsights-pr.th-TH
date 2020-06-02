---
title: 1385-Office-365-การแจ้งเตือน-นโยบาย
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502446"
---
# <a name="alert-policies"></a><span data-ttu-id="dcea0-102">นโยบายการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="dcea0-102">Alert policies</span></span>

<span data-ttu-id="dcea0-103">ศูนย์การปฏิบัติตามกฎระเบียบ& Microsoft 365 มี[นโยบายการแจ้งเตือนเริ่มต้น](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)ที่ทริกเกอร์การแจ้งเตือนสําหรับองค์กรที่มี Office 365 องค์กรหรือ Office 365 รัฐบาลสหรัฐ E1/G1, E3/G3 หรือ E5/G5 การสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="dcea0-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="dcea0-104">ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลที่ส่งโดยOffice365Alerts@microsoft.comกับบรรทัดเรื่องเช่น "การแจ้งเตือนความรุนแรงต่ํา:*ชื่อของนโยบายการแจ้งเตือน*"</span><span class="sxs-lookup"><span data-stu-id="dcea0-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="dcea0-105">การแจ้งเตือนจะถูกส่งเมื่อมีการทริกเกอร์การแจ้งเตือนสําหรับกิจกรรมทั่วไป เช่น เมื่อผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="dcea0-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="dcea0-106">สร้างกฎของกล่องขาเข้าที่ส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="dcea0-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="dcea0-107">กําหนดสิทธิ์ในกล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="dcea0-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="dcea0-108">แชร์หรือลบแฟ้มจํานวนมากในการแชร์ไฟล์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="dcea0-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="dcea0-109">สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="dcea0-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="dcea0-110">วิธีตรวจสอบและดําเนินการกับการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="dcea0-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="dcea0-111">ไปที่[ศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย](https://protection.office.com)และลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="dcea0-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="dcea0-112">คลิก**Alerts**  >  **การแจ้งเตือนมุมมอง**การแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="dcea0-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="dcea0-113">คลิกการแจ้งเตือนเพื่อแสดงหน้าลอยพร้อมข้อมูลเกี่ยวกับการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="dcea0-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="dcea0-114">คุณสามารถดําเนินการกับการแจ้งเตือน เช่น[การลบกฎกล่องจดหมายที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)</span><span class="sxs-lookup"><span data-stu-id="dcea0-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="dcea0-115">หรือคุณสามารถปิดการแจ้งเตือนได้โดยคลิก**แก้ไข**ในหน้าการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="dcea0-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="dcea0-116">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าคอนฟิกและการจัดการนโยบายการแจ้งเตือน ให้ดูที่[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)</span><span class="sxs-lookup"><span data-stu-id="dcea0-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="dcea0-117">**สําคัญ**: การแจ้งเตือนอีเมลแจ้งเตือนจาก Microsoft จะไม่ขอให้คุณทําสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="dcea0-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="dcea0-118">ใส่รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="dcea0-118">Provide a password</span></span>
- <span data-ttu-id="dcea0-119">ยืนยันรายละเอียดความปลอดภัยของบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="dcea0-119">Verify the security details of your account</span></span>
- <span data-ttu-id="dcea0-120">ตรวจสอบตัวตนใหม่ด้วยตัวคุณเอง</span><span class="sxs-lookup"><span data-stu-id="dcea0-120">Re-authenticate yourself</span></span>

<span data-ttu-id="dcea0-121">หากคุณได้รับข้อความอีเมลเช่นนี้ Microsoft จะไม่ถูกส่งมา และควรได้รับการพิจารณาว่าเป็นฟิชชิ่ง</span><span class="sxs-lookup"><span data-stu-id="dcea0-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="dcea0-122">หากเกิดเหตุการณ์ดังกล่าวโปรด[รายงานไปยัง Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)</span><span class="sxs-lookup"><span data-stu-id="dcea0-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>