---
title: แฟ้มบันทึกและการรายงาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036098"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="16212-102">แฟ้มบันทึกและการรายงาน</span><span class="sxs-lookup"><span data-stu-id="16212-102">Logs and Reporting</span></span>

<span data-ttu-id="16212-103">[คําตอบที่ถามบ่อยเกี่ยวกับ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) การรายงาน Azure Active Directory (Azure AD) ของการรายงานของ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="16212-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="16212-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="16212-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="16212-105">**การแก้ไขปัญหาเกี่ยวกับการตรวจสอบ**</span><span class="sxs-lookup"><span data-stu-id="16212-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="16212-106">หากคุณมีปัญหาในการดูกิจกรรมการตรวจสอบบางอย่างและกิจกรรมที่หายไปอยู่ใน [รายการนี้](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)โปรดส่งตั๋วการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="16212-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="16212-107">ถ้าคุณมีปัญหาในการดูบันทึกการตรวจสอบใดๆ ในผู้เช่าของคุณ โปรดส่งตั๋วการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="16212-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="16212-108">ถ้ากิจกรรมการตรวจสอบของคุณไม่แสดงขึ้นทันทีในพอร์ทัล Azure ให้ตรวจสอบข้อมูลเวลาแฝงของเรา[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)และจัดเก็บตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงที่บันทึก</span><span class="sxs-lookup"><span data-stu-id="16212-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="16212-109">การเก็บข้อมูลบันทึกกิจกรรม Azure AD</span><span class="sxs-lookup"><span data-stu-id="16212-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="16212-110">ถ้าคุณไม่เห็นการตรวจสอบทั้งหมดในช่วงวันที่ที่คุณเลือก คุณสามารถดาวน์โหลดแถวได้มากถึง 250K (เรียงล>บตามล>นล่าสุด) ของการลงชื่อเข้าใช้จากพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="16212-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="16212-111">หากต้องการข้อมูลเพิ่มเติม โปรดดู[การดาวน์โหลดกิจกรรมการตรวจสอบ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="16212-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="16212-112">**การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้**</span><span class="sxs-lookup"><span data-stu-id="16212-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="16212-113">คุณสามารถดูข้อมูลได้เพียง 30 วันสุดท้ายถ้าคุณมีสิทธิ์การใช้งาน Azure AD Premium (P1 หรือ P2) ของผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="16212-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="16212-114">การลงชื่อเข้าใช้จะพร้อมใช้งานเฉพาะกับผู้เช่า Azure AD Premium เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="16212-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="16212-115">ซึ่งไม่มีให้ใช้งานในผู้เช่าที่มีสิทธิ์การใช้งานแบบฟรีหรือแบบพื้นฐาน</span><span class="sxs-lookup"><span data-stu-id="16212-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="16212-116">ถ้าผู้เช่าของคุณมีสิทธิ์การใช้งาน P1 แบบพรีเมียม และคุณไม่สามารถดูการลงชื่อเข้าใช้ ให้ดูข้อมูลเวลาแฝงของเรา[](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)และเปิดไฟล์ตั๋วการสนับสนุนถ้าความล่าช้าเกินเวลาแฝงของเอกสาร</span><span class="sxs-lookup"><span data-stu-id="16212-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="16212-117">ถ้าคุณไม่เห็นการลงชื่อเข้าใช้ทั้งหมดในช่วงวันที่ที่คุณเลือก โปรดสังเกตว่าคุณสามารถดาวน์โหลดแถวได้ถึง 250K (เรียงล>บตามล่าสุด) ของการลงชื่อเข้าใช้จากพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="16212-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="16212-118">หากต้องการข้อมูลเพิ่มเติม [โปรดดูการดาวน์โหลดกิจกรรมการ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)ลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="16212-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="16212-119">**แก้ไขปัญหารายงานความปลอดภัย (ผู้ใช้ที่ถูกตั้งค่าสถานะที่มีความเสี่ยง การลงชื่อเข้าใช้ที่มีความเสี่ยง)**</span><span class="sxs-lookup"><span data-stu-id="16212-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="16212-120">ผู้ใช้ที่ถูกตั้งค่าสถานะรายงานด้านความปลอดภัยของความเสี่ยง</span><span class="sxs-lookup"><span data-stu-id="16212-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="16212-121">รายงานการลงชื่อเข้าใช้ที่มีความเสี่ยงในพอร์ทัล Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="16212-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="16212-122">เหตุการณ์ความเสี่ยง Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="16212-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
