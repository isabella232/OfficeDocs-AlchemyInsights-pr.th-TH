---
title: อัปเดตรายละเอียดการชำระเงินใน Azure (สมัยใหม่)
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9003546"
- "6857"
ms.openlocfilehash: bb032f772077318e54ac4fde42a72f432703d828
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807880"
---
# <a name="update-payment-details-in-azure"></a><span data-ttu-id="1fd83-102">อัปเดตรายละเอียดการชำระเงินใน Azure</span><span class="sxs-lookup"><span data-stu-id="1fd83-102">Update payment details in Azure</span></span>

<span data-ttu-id="1fd83-103">ถ้าบัตรเครดิตของคุณได้รับการต่ออายุและหมายเลขยังคงเหมือนเดิมให้อัปเดตรายละเอียดบัตรเครดิตที่มีอยู่เช่นวันหมดอายุ</span><span class="sxs-lookup"><span data-stu-id="1fd83-103">If your credit card gets renewed and the number stays the same, update the existing credit card details like the expiration date.</span></span> <span data-ttu-id="1fd83-104">ถ้าหมายเลขบัตรเครดิตของคุณเปลี่ยนไปเนื่องจากบัตรสูญหายถูกขโมยหรือหมดอายุให้ทำตามขั้นตอนในส่วน[เพิ่มบัตรเครดิตเป็นวิธีการชำระเงิน](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard)</span><span class="sxs-lookup"><span data-stu-id="1fd83-104">If your credit card number changes because the card is lost, stolen, or expired, follow the steps in the [Add a credit card as a payment method](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) section.</span></span> <span data-ttu-id="1fd83-105">คุณไม่จำเป็นต้องอัปเด CVV</span><span class="sxs-lookup"><span data-stu-id="1fd83-105">You don't need to update the CVV.</span></span>

<span data-ttu-id="1fd83-106">วิธีการชำระเงินของคุณเชื่อมโยงกับ[โปรไฟล์การเรียกเก็บเงิน](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile)</span><span class="sxs-lookup"><span data-stu-id="1fd83-106">Your Payment methods are associated with [billing profiles](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span></span> <span data-ttu-id="1fd83-107">เฉพาะผู้ใช้ที่ลงทะเบียนสำหรับ Azure และสร้างบัญชีผู้ใช้การเรียกเก็บเงินเท่านั้นที่สามารถอัปเดตวิธีการชำระเงินได้</span><span class="sxs-lookup"><span data-stu-id="1fd83-107">Only the user who signed up for Azure and created the billing account can update the payment method.</span></span> <span data-ttu-id="1fd83-108">ทำตามขั้นตอนต่อไปนี้เพื่ออัปเดตวิธีการชำระเงิน</span><span class="sxs-lookup"><span data-stu-id="1fd83-108">Follow these steps to update the payment method.</span></span>

1. <span data-ttu-id="1fd83-109">ลงชื่อเข้าใช้[พอร์ทัล Azure](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="1fd83-109">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="1fd83-110">ค้นหา **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="1fd83-110">Search on **Cost Management + Billing** .</span></span>

3. <span data-ttu-id="1fd83-111">ในเมนูทางด้านซ้ายให้เลือก **โปรไฟล์การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="1fd83-111">In the menu on the left, select **Billing profiles** .</span></span>

4. <span data-ttu-id="1fd83-112">เลือกโปรไฟล์การเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="1fd83-112">Select a billing profile.</span></span>

5. <span data-ttu-id="1fd83-113">ในเมนูทางด้านซ้ายให้เลือก **วิธีการชำระเงิน**</span><span class="sxs-lookup"><span data-stu-id="1fd83-113">In the menu on the left, select **Payment methods** .</span></span>

6. <span data-ttu-id="1fd83-114">ในส่วน **บัตรเครดิตของคุณ** ให้ค้นหาบัตรเครดิตที่คุณต้องการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="1fd83-114">In the **Your credit cards** section, find the credit card you want to edit.</span></span>
7. <span data-ttu-id="1fd83-115">เลือกจุดไข่ปลา **(...)** ที่ส่วนท้ายของแถว</span><span class="sxs-lookup"><span data-stu-id="1fd83-115">Select the ellipsis **(...)** at the end of the row.</span></span>

8. <span data-ttu-id="1fd83-116">เมื่อต้องการแก้ไขรายละเอียดบัตรเครดิตของคุณให้เลือก  **แก้ไข**  จากเมนูบริบท</span><span class="sxs-lookup"><span data-stu-id="1fd83-116">To edit your credit card details, select  **Edit**  from the context menu.</span></span>
