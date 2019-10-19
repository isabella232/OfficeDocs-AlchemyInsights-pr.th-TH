---
title: ไม่มีการส่งการแจ้งเตือนการแจ้งเตือนของ SharePoint
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36744660"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="59b2a-102">ไม่มีการส่งการแจ้งเตือนการแจ้งเตือนของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="59b2a-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="59b2a-103">กรุณาตรวจสอบโฟลเดอร์ขยะใน e-mail ของคุณเป็นบางครั้งการแจ้งเตือนอาจจะไปที่นั่น</span><span class="sxs-lookup"><span data-stu-id="59b2a-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="59b2a-104">ตรวจสอบว่าไม่มีการจัดส่งการ**แจ้งเตือนทั้งหมด**หรือถ้าไม่มี**การส่งการแจ้งเตือนแต่ละรายการ**จากแฟ้มหรือไลบรารีเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="59b2a-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="59b2a-105">การ**แจ้งเตือนแต่ละครั้งจะไม่มีการจัดส่ง**: ถ้าไม่มีการส่งการแจ้งเตือนแต่ละรายการจากแฟ้มหรือไลบรารีที่ระบุคุณสามารถพยายามลบและสร้างขึ้นใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="59b2a-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="59b2a-106">ดู[จัดการดูหรือลบการแจ้งเตือนของ SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online)เพื่อสร้างการแจ้งเตือนใหม่</span><span class="sxs-lookup"><span data-stu-id="59b2a-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="59b2a-107">การ**แจ้งเตือนทั้งหมดจะไม่ถูกส่ง**: ถ้าการแจ้งเตือนทั้งหมดจากหลายไฟล์หรือไลบรารีจะไม่ถูกส่งไปที่[แดชบอร์ดความสมบูรณ์ของบริการ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)เพื่อตรวจสอบคำแนะนำ/เหตุการณ์ที่อาจเกิดขึ้นกับ SharePoint หรือ Exchange</span><span class="sxs-lookup"><span data-stu-id="59b2a-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="59b2a-108">ปัญหานี้อาจจะมีความสามารถในการแจ้งเตือนของ SharePoint หรือล่าช้าในการส่งผ่านการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="59b2a-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="59b2a-109">นอกจากนี้ยังจะเป็นสิ่งสำคัญที่จะทราบว่ามีการจัดส่งทาง e-mail อื่นๆและถ้าไม่ปัญหาที่มีแนวโน้มที่จะเกิดความล่าช้าของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="59b2a-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="59b2a-110">คำถามที่พบบ่อยเกี่ยวกับการแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="59b2a-110">FAQ on alerts:</span></span>

- <span data-ttu-id="59b2a-111">ไม่สามารถส่งการแจ้งเตือนไปยังกลุ่มการแจกจ่ายได้สนับสนุนเฉพาะกลุ่มการรักษาความปลอดภัยและ O365 เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="59b2a-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="59b2a-112">คุณไม่สามารถกำหนดเทมเพลตอีเมลแจ้งเตือนได้ คุณจำเป็นต้องใช้ Microsoft FLOW หรือ SharePoint Designer เวิร์กโฟลว์เพื่อให้บรรลุเป้าหมายเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="59b2a-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="59b2a-113">ข้อมูลเพิ่มเติม:</span><span class="sxs-lookup"><span data-stu-id="59b2a-113">More Information:</span></span>

- <span data-ttu-id="59b2a-114">**การตั้งค่าการแจ้งเตือน**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนโปรดดูที่การสร้างการแจ้ง[เตือนเพื่อรับการแจ้งให้ทราบเมื่อมีการเปลี่ยนแปลงแฟ้มหรือโฟลเดอร์ใน SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)</span><span class="sxs-lookup"><span data-stu-id="59b2a-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="59b2a-115">**แก้ไขปัญหาการแจ้งเตือน**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการแก้ไขปัญหาการแจ้งเตือนให้ดูที่[ผู้ใช้ไม่ได้รับการแจ้งเตือนของ SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)</span><span class="sxs-lookup"><span data-stu-id="59b2a-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="59b2a-116">**นโยบายการแจ้งเตือนการปฏิบัติตามกฎระเบียบของ O365 ขั้นสูง**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าการแจ้งเตือนเหล่านี้โปรดดูที่[นโยบายการแจ้งเตือนการปฏิบัติตามนโยบาย](https://docs.microsoft.com/office365/securitycompliance/alert-policies)</span><span class="sxs-lookup"><span data-stu-id="59b2a-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="59b2a-117">**บันทึกการตรวจสอบ SharePoint และ OneDrive**: สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการกู้คืนเหตุการณ์เหล่านี้โปรดดู[ที่การค้นหาบันทึกการตรวจสอบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)</span><span class="sxs-lookup"><span data-stu-id="59b2a-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="59b2a-118">ข้อความ**แจ้งเตือนที่ส่งโดยการป้องกันภัยคุกคามขั้นสูง**: ดู[ATP สำหรับ SharePoint และ OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="59b2a-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="59b2a-119">ข้อความ**แจ้งเตือนที่ส่งโดยนโยบายการป้องกันการสูญหายของข้อมูล**: ดู[การแจ้งเตือนทางเมลให้กับกรมธรรม์ DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="59b2a-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="59b2a-120">หัวข้อที่เกี่ยวข้อง</span><span class="sxs-lookup"><span data-stu-id="59b2a-120">Related Topics</span></span>

<span data-ttu-id="59b2a-121">ต้องการลองการไหลของ Microsoft ใน SharePoint แบบออนไลน์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="59b2a-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="59b2a-122">สร้างโฟลว์</span><span class="sxs-lookup"><span data-stu-id="59b2a-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="59b2a-123">SharePoint และการไหล</span><span class="sxs-lookup"><span data-stu-id="59b2a-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
