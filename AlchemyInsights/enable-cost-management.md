---
title: เปิดใช้งานการจัดการต้นทุน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678774"
---
# <a name="enable-cost-management"></a><span data-ttu-id="f882d-102">เปิดใช้งานการจัดการต้นทุน</span><span class="sxs-lookup"><span data-stu-id="f882d-102">Enable cost management</span></span>

<span data-ttu-id="f882d-103">**' ค่าใช้จ่าย ' ถูกปิดใช้งานสำหรับองค์กรของคุณอย่างไร**</span><span class="sxs-lookup"><span data-stu-id="f882d-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="f882d-104">องค์กรที่ใช้บัญชีข้อตกลงขององค์กร (EA) หรือบัญชีผู้ใช้ข้อตกลงลูกค้าของ Microsoft (MCA) สามารถปิดใช้งานการเข้าถึงข้อมูลต้นทุนและข้อมูลการกำหนดราคาได้</span><span class="sxs-lookup"><span data-stu-id="f882d-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="f882d-105">หลังจากที่คุณเข้าสู่ระบบไปยังพอร์ทัล Azure พวกเขาสามารถใช้ APIs การเรียกเก็บเงินเพื่อรับใบแจ้งหนี้ได้โดยทางโปรแกรม (เมื่อมีการเข้าร่วม) และรายละเอียดการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f882d-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="f882d-106">**วิธีการอนุญาตให้ผู้ใช้เพิ่มเติมในการเข้าถึงใบแจ้งหนี้**</span><span class="sxs-lookup"><span data-stu-id="f882d-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="f882d-107">ไปที่ **ใบมีดการสมัคร** ใช้งานในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="f882d-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="f882d-108">เลือก **ใบแจ้งหนี้** แล้ว **เข้าถึงใบแจ้งหนี้**</span><span class="sxs-lookup"><span data-stu-id="f882d-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="f882d-109">เปิดใช้งานการเข้าถึงตามด้วยการบันทึกการเปลี่ยนแปลงเพื่ออนุญาตให้ผู้ใช้ในการสมัครใช้งาน-ลักษณะบทบาทในการดาวน์โหลดใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="f882d-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="f882d-110">ผู้ดูแลระบบบัญชียังสามารถกำหนดค่าให้มีใบแจ้งหนี้ที่ส่งผ่านทางอีเมล</span><span class="sxs-lookup"><span data-stu-id="f882d-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="f882d-111">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[รับใบแจ้งหนี้ของคุณในอีเมล](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)</span><span class="sxs-lookup"><span data-stu-id="f882d-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="f882d-112">**วิธีเพิ่มผู้ใช้ลงในบทบาทผู้อ่านการเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="f882d-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="f882d-113">ไปที่ **ใบมีดการสมัคร** ใช้งานในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="f882d-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="f882d-114">เลือก **ตัวควบคุมการเข้าถึง (IAM)** แล้วคลิก **เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="f882d-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="f882d-115">เลือกตัว **อ่านการเรียกเก็บเงิน** ในหน้า **เลือกบทบาท**</span><span class="sxs-lookup"><span data-stu-id="f882d-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="f882d-116">พิมพ์อีเมลของผู้ใช้ที่คุณต้องการเชิญแล้วคลิก **ตกลง** เพื่อส่งคำเชิญ</span><span class="sxs-lookup"><span data-stu-id="f882d-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="f882d-117">ทำตามคำแนะนำที่ให้ไว้ในอีเมลเชิญเพื่อเข้าสู่ระบบในฐานะผู้อ่านการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="f882d-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="f882d-118">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ให้สิทธิ์การเข้าถึงการเรียกเก็บเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)</span><span class="sxs-lookup"><span data-stu-id="f882d-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="f882d-119">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="f882d-119">**Recommended documents**</span></span>

- [<span data-ttu-id="f882d-120">เปิดใช้งานมุมมอง DA และอ่าวผ่านทาง EA portal</span><span class="sxs-lookup"><span data-stu-id="f882d-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="f882d-121">ค่าใช้จ่ายที่รวมอยู่ในการจัดการต้นทุน</span><span class="sxs-lookup"><span data-stu-id="f882d-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="f882d-122">ข้อเสนอ Microsoft Azure ที่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="f882d-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="f882d-123">ตรวจทานต้นทุนในการวิเคราะห์ต้นทุน</span><span class="sxs-lookup"><span data-stu-id="f882d-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="f882d-124">ให้สิทธิ์การเข้าถึงข้อมูลการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="f882d-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f882d-125">ตรวจสอบการเข้าถึงข้อตกลงลูกค้าของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="f882d-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






