---
title: การออกใบแจ้งหนี้อีเมล Azure สมัยใหม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922146"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="f4202-102">การออกใบแจ้งหนี้ทางอีเมลใน Azure</span><span class="sxs-lookup"><span data-stu-id="f4202-102">Email invoicing in Azure</span></span>

<span data-ttu-id="f4202-103">คุณต้องมีเจ้าของหรือบทบาทผู้สนับสนุนบนโปรไฟล์การเรียกเก็บเงินหรือบัญชีผู้ใช้การเรียกเก็บเงินเพื่ออัปเดตการกำหนดลักษณะใบแจ้งหนี้ของอีเมล</span><span class="sxs-lookup"><span data-stu-id="f4202-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="f4202-104">เมื่อคุณเข้าร่วมการเข้าร่วมผู้ใช้ทั้งหมดที่มีบทบาทผู้สนับสนุนผู้อ่านและผู้จัดการใบแจ้งหนี้ในโปรไฟล์การเรียกเก็บเงินจะได้รับใบแจ้งหนี้ในอีเมล</span><span class="sxs-lookup"><span data-stu-id="f4202-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="f4202-105">ลงชื่อเข้าใช้[พอร์ทัล Azure](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="f4202-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f4202-106">ค้นหา **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="f4202-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="f4202-107">เลือก **ใบแจ้งหนี้** จากด้านซ้ายมือแล้วเลือก **ใบแจ้งหนี้ทางอีเม** ลจากด้านบนของหน้า</span><span class="sxs-lookup"><span data-stu-id="f4202-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="f4202-108">ถ้าคุณมีโปรไฟล์การเรียกเก็บเงินหลายโปรไฟล์ให้เลือกโปรไฟล์การเรียกเก็บเงินแล้วเลือก **เลือกเข้า** ร่วม</span><span class="sxs-lookup"><span data-stu-id="f4202-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="f4202-109">เลือก **อัปเดต**</span><span class="sxs-lookup"><span data-stu-id="f4202-109">Select **Update**.</span></span>
6. <span data-ttu-id="f4202-110">ถ้าคุณมีโปรไฟล์การเรียกเก็บเงินหลายโปรไฟล์ให้เลือกโปรไฟล์การเรียกเก็บเงินแล้วเลือก **เลือกเข้า** ร่วม</span><span class="sxs-lookup"><span data-stu-id="f4202-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="f4202-111">คุณให้ผู้อื่นเข้าถึงมุมมองดาวน์โหลดและชำระเงินในใบแจ้งหนี้โดยการกำหนดบทบาทผู้จัดการใบแจ้งหนี้สำหรับโปรไฟล์การเรียกเก็บเงิน MCA หรือ MPA</span><span class="sxs-lookup"><span data-stu-id="f4202-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="f4202-112">ถ้าคุณได้เลือกที่จะรับใบแจ้งหนี้ของคุณในอีเมลผู้ใช้จะได้รับใบแจ้งหนี้ในอีเมล</span><span class="sxs-lookup"><span data-stu-id="f4202-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="f4202-113">ลงชื่อเข้าใช้[พอร์ทัล Azure](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="f4202-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f4202-114">ค้นหา **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="f4202-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="f4202-115">เลือก **โปรไฟล์การเรียกเก็บเงิน** จากด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="f4202-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="f4202-116">จากรายการโปรไฟล์การเรียกเก็บเงินให้เลือกโปรไฟล์การเรียกเก็บเงินที่คุณต้องการกำหนดบทบาทผู้จัดการใบแจ้งหนี้</span><span class="sxs-lookup"><span data-stu-id="f4202-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="f4202-117">เลือก **ตัวควบคุมการเข้าถึง (IAM)** จากด้านซ้ายมือแล้วเลือก **เพิ่ม** จากด้านบนของหน้า</span><span class="sxs-lookup"><span data-stu-id="f4202-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="f4202-118">ในรายการดรอปดาวน์บทบาทให้เลือก **ตัวจัดการใบแจ้งหนี้**</span><span class="sxs-lookup"><span data-stu-id="f4202-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="f4202-119">ใส่ที่อยู่อีเมลของผู้ใช้เพื่อให้สิทธิ์การเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="f4202-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="f4202-120">เลือก **บันทึก** เพื่อกำหนดบทบาท</span><span class="sxs-lookup"><span data-stu-id="f4202-120">Select **Save** to assign the role.</span></span>
