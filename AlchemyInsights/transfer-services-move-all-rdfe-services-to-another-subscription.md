---
title: บริการถ่ายโอน-ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692179"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="e8649-102">บริการถ่ายโอน-ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น</span><span class="sxs-lookup"><span data-stu-id="e8649-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="e8649-103">**ย้ายทรัพยากร**</span><span class="sxs-lookup"><span data-stu-id="e8649-103">**Move resources**</span></span>

<span data-ttu-id="e8649-104">ทรัพยากร azure สามารถย้ายไปยังการสมัครใช้งาน Azure หรือกลุ่มทรัพยากรอื่นภายใต้การสมัครใช้งานเดียวกันได้โดยใช้ Azure portal, Azure PowerShell, Azure CLI หรือส่วนที่เหลือ API เพื่อย้ายทรัพยากร</span><span class="sxs-lookup"><span data-stu-id="e8649-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="e8649-105">ก่อนที่คุณจะสามารถย้ายแหล่งข้อมูลให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="e8649-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="e8649-106">รายการตรวจสอบก่อนที่จะย้ายทรัพยากร</span><span class="sxs-lookup"><span data-stu-id="e8649-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="e8649-107">บริการที่สามารถย้ายได้</span><span class="sxs-lookup"><span data-stu-id="e8649-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="e8649-108">วิธีตรวจสอบความถูกต้องของการย้าย</span><span class="sxs-lookup"><span data-stu-id="e8649-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="e8649-109">ย้ายคำแนะนำสำหรับบริการ</span><span class="sxs-lookup"><span data-stu-id="e8649-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="e8649-110">เมื่อต้องการย้ายแหล่งข้อมูลที่มีอยู่ไปยังกลุ่มทรัพยากรอื่นหรือการสมัครใช้งานคุณสามารถใช้:</span><span class="sxs-lookup"><span data-stu-id="e8649-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="e8649-111">พอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="e8649-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="e8649-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8649-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="e8649-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e8649-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="e8649-114">REST API</span><span class="sxs-lookup"><span data-stu-id="e8649-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="e8649-115">บทช่วยสอน:[ย้ายทรัพยากร Azure ไปยังกลุ่มทรัพยากรอื่นหรือการสมัคร](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)ใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e8649-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="e8649-116">**การแก้ไขปัญหาข้อผิดพลาดด้วยตัวจัดการทรัพยากร Azure**</span><span class="sxs-lookup"><span data-stu-id="e8649-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="e8649-117">ดูบทความด้านล่างนี้เพื่อเรียนรู้เกี่ยวกับข้อผิดพลาดในการปรับใช้ Azure ทั่วไปและรับข้อมูลเพื่อแก้ไขปัญหาเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="e8649-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="e8649-118">ถ้าคุณไม่พบรหัสข้อผิดพลาดสำหรับข้อผิดพลาดในการปรับใช้ของคุณให้ดูที่[ค้นหารหัสข้อผิดพลาด](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)</span><span class="sxs-lookup"><span data-stu-id="e8649-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="e8649-119">การแก้ไขปัญหาข้อผิดพลาดในการปรับใช้</span><span class="sxs-lookup"><span data-stu-id="e8649-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="e8649-120">การแก้ไขปัญหาการย้ายทรัพยากร Azure ไปยังกลุ่มทรัพยากรใหม่หรือการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e8649-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="e8649-121">โปรดทราบว่าถ้าคุณต้องการอัปเกรดการสมัครใช้งาน Azure ของคุณเช่นการสลับจากค่าใช้จ่ายที่ไม่มีค่าใช้จ่ายในขณะเดินทางคุณจะต้องแปลงการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="e8649-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="e8649-122">เมื่อต้องการอัปเกรดเวอร์ชันทดลองใช้ฟรีให้ดูที่[อัปเกรดเวอร์ชันทดลองใช้ฟรีของคุณหรือ Microsoft ลองใช้การสมัครใช้งาน Azure เพื่อชำระเงินตามที่คุณไป](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="e8649-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="e8649-123">เมื่อต้องการเปลี่ยนบัญชีผู้ใช้แบบชำระเงินเป็นแบบของคุณให้ดูที่[เปลี่ยนการสมัครใช้งานแบบชำระเงินของ Azure ของคุณไปยังข้อเสนออื่น](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)</span><span class="sxs-lookup"><span data-stu-id="e8649-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="e8649-124">**เมื่อต้องการเพิ่มหรือเชื่อมโยงการสมัครใช้งาน Azure กับผู้เช่า Azure Active directory ของคุณให้ทำดังนี้**</span><span class="sxs-lookup"><span data-stu-id="e8649-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="e8649-125">ลงชื่อเข้าใช้และเลือกการสมัครใช้งานที่คุณต้องการใช้จากหน้าการสมัครใช้งาน[ใน Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="e8649-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="e8649-126">เลือก **เปลี่ยนไดเรกทอรี**</span><span class="sxs-lookup"><span data-stu-id="e8649-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="e8649-127">ตรวจทานคำเตือนที่ปรากฏขึ้นจากนั้นเลือก **เปลี่ยน**</span><span class="sxs-lookup"><span data-stu-id="e8649-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="e8649-128">ไดเรกทอรีจะถูกเปลี่ยนแปลงสำหรับการสมัครใช้งานและคุณจะได้รับข้อความแสดงความสำเร็จ</span><span class="sxs-lookup"><span data-stu-id="e8649-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="e8649-129">ใช้ตัวสลับ *ไดเรกทอรี* เพื่อไปที่ไดเรกทอรีใหม่ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e8649-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="e8649-130">อาจใช้เวลาถึง10นาทีเพื่อให้ทุกอย่างแสดงได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="e8649-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="e8649-131">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="e8649-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="e8649-132">การโอนความเป็นเจ้าของการสมัครใช้งาน Azure</span><span class="sxs-lookup"><span data-stu-id="e8649-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="e8649-133">ย้ายทรัพยากรไปยังกลุ่มทรัพยากรใหม่หรือการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e8649-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="e8649-134">จัดการทรัพยากรโดยใช้พอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="e8649-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
