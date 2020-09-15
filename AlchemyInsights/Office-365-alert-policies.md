---
title: ๑๓๘๕-Office-๓๖๕-การแจ้งเตือน-นโยบาย
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664045"
---
# <a name="alert-policies"></a><span data-ttu-id="37d9d-102">นโยบายการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="37d9d-102">Alert policies</span></span>

<span data-ttu-id="37d9d-103">ศูนย์การรักษาความปลอดภัย & ของ Microsoft ๓๖๕มี [นโยบายการแจ้งเตือนเริ่มต้น](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) ที่ทริกเกอร์การแจ้งเตือนสำหรับองค์กรที่มี Office ๓๖๕ Enterprise หรือ Office ๓๖๕สหรัฐอเมริการัฐ E1/G1, E3/G3 หรือการสมัครใช้งานแบบ E5/G5/G5</span><span class="sxs-lookup"><span data-stu-id="37d9d-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="37d9d-104">ผู้ดูแลระบบอาจได้รับการแจ้งเตือนทางอีเมลการแจ้งเตือนที่ส่งโดย Office365Alerts@microsoft.com กับบรรทัดชื่อเรื่องเช่น "การแจ้งเตือนความรุนแรงต่ำ: *ชื่อของนโยบายการแจ้งเตือน*"</span><span class="sxs-lookup"><span data-stu-id="37d9d-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="37d9d-105">การแจ้งเตือนจะถูกส่งเมื่อข้อความแจ้งเตือนถูกทริกเกอร์สำหรับกิจกรรมทั่วไปเช่นเมื่อผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="37d9d-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="37d9d-106">สร้างกฎกล่องจดหมายเข้าที่ส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="37d9d-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="37d9d-107">กำหนดสิทธิ์กล่องจดหมายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="37d9d-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="37d9d-108">แชร์หรือลบไฟล์จำนวนมากในการแชร์ไฟล์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="37d9d-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="37d9d-109">สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="37d9d-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="37d9d-110">เมื่อต้องการตรวจสอบและดำเนินการกับการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="37d9d-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="37d9d-111">ไปที่ [ศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย](https://protection.office.com) และลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="37d9d-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="37d9d-112">คลิ**กการแจ้งเตือน**  >  **มุมมอง**การแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="37d9d-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="37d9d-113">คลิกที่การแจ้งเตือนเพื่อแสดงหน้าลอยที่มีข้อมูลเกี่ยวกับการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="37d9d-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="37d9d-114">คุณสามารถดำเนินการกับการแจ้งเตือนเช่นการ [เอากฎกล่องจดหมายเข้าที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)ออก</span><span class="sxs-lookup"><span data-stu-id="37d9d-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="37d9d-115">หรือคุณก็สามารถปิดการแจ้งเตือนได้โดยการคลิก **แก้ไข** บนหน้าเมนูลอยตัวของการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="37d9d-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="37d9d-116">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดค่าและการจัดการนโยบายการแจ้งเตือนให้ดู[บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)</span><span class="sxs-lookup"><span data-stu-id="37d9d-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="37d9d-117">**สิ่งสำคัญ**: การแจ้งเตือนทางอีเมลที่แจ้งเตือนจาก Microsoft จะไม่ขอให้คุณทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="37d9d-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="37d9d-118">ใส่รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="37d9d-118">Provide a password</span></span>
- <span data-ttu-id="37d9d-119">ตรวจสอบรายละเอียดความปลอดภัยของบัญชีผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="37d9d-119">Verify the security details of your account</span></span>
- <span data-ttu-id="37d9d-120">การรับรองความถูกต้องอีกครั้งด้วยตัวคุณเอง</span><span class="sxs-lookup"><span data-stu-id="37d9d-120">Re-authenticate yourself</span></span>

<span data-ttu-id="37d9d-121">ถ้าคุณได้รับข้อความอีเมลที่มีข้อความนี้ไม่ได้ถูกส่งโดยไมโครซอฟท์และควรถือว่าเป็นการหลอกลวงฟิชชิ่ง</span><span class="sxs-lookup"><span data-stu-id="37d9d-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="37d9d-122">ถ้าเกิดเหตุการณ์ดังกล่าวโปรด[รายงานข้อมูลนั้นไปยังไมโครซอฟท์](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)</span><span class="sxs-lookup"><span data-stu-id="37d9d-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>