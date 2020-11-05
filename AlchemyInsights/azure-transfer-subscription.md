---
title: โอนสิทธิ์การเรียกเก็บเงิน Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922172"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="ac6ac-102">โอนสิทธิ์การเรียกเก็บเงิน Azure</span><span class="sxs-lookup"><span data-stu-id="ac6ac-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="ac6ac-103">ลงชื่อเข้าใช้ [พอร์ทัล Azure](https://portal.azure.com/) ในฐานะผู้ดูแลระบบของบัญชีผู้ใช้การเรียกเก็บเงินที่มีการสมัครใช้งานที่คุณต้องการโอนย้าย</span><span class="sxs-lookup"><span data-stu-id="ac6ac-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="ac6ac-104">ถ้าคุณไม่แน่ใจว่าคุณเป็นผู้ดูแลระบบหรือไม่หรือถ้าคุณต้องการกำหนดใครให้ดูที่[กำหนดผู้ดูแลการเรียกเก็บเงินของบัญชีผู้ใช้](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)</span><span class="sxs-lookup"><span data-stu-id="ac6ac-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="ac6ac-105">ค้นหา **การจัดการต้นทุน + การเรียกเก็บเงิน**</span><span class="sxs-lookup"><span data-stu-id="ac6ac-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="ac6ac-106">เลือกการ **สมัคร** ใช้งานจากบานหน้าต่างด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="ac6ac-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="ac6ac-107">คุณอาจจำเป็นต้องเลือกขอบเขตการเรียกเก็บเงินจากนั้นการ **สมัคร** ใช้งานหรือการสมัครใช้งาน **Azure** ทั้งนี้ขึ้นอยู่กับการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="ac6ac-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="ac6ac-108">เลือก **โอนความเป็นเจ้าของการเรียกเก็บเงิน** สำหรับการสมัครใช้งานที่คุณต้องการโอนย้าย</span><span class="sxs-lookup"><span data-stu-id="ac6ac-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="ac6ac-109">ใส่ที่อยู่อีเมลของผู้ใช้ที่เป็นผู้ดูแลการเรียกเก็บเงินของบัญชีผู้ใช้ที่จะเป็นเจ้าของใหม่สำหรับการสมัครใช้งานแล้วเลือก **ส่งคำขอการโอนย้าย**</span><span class="sxs-lookup"><span data-stu-id="ac6ac-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="ac6ac-110">ผู้ใช้ได้รับอีเมลที่มีคำแนะนำในการตรวจสอบคำขอการโอนย้ายของคุณ</span><span class="sxs-lookup"><span data-stu-id="ac6ac-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="ac6ac-111">เมื่อต้องการอนุมัติคำขอการโอนย้ายผู้ใช้จะเลือกลิงก์ในอีเมลและตามคำแนะนำ</span><span class="sxs-lookup"><span data-stu-id="ac6ac-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="ac6ac-112">**หมายเหตุ** : ถ้าคุณโอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งานของคุณไปยังบัญชีผู้ใช้ของคุณในผู้เช่า Azure AD อื่นการมอบหมายการ [ควบคุมการเข้าถึงตามบทบาท (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)ทั้งหมดเพื่อจัดการทรัพยากรในการสมัครใช้งานจะถูกเอาออกอย่างถาวร</span><span class="sxs-lookup"><span data-stu-id="ac6ac-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="ac6ac-113">เฉพาะเจ้าของใหม่เท่านั้นที่จะมีสิทธิ์เข้าถึงเพื่อจัดการทรัพยากรในการสมัครใช้งาน</span><span class="sxs-lookup"><span data-stu-id="ac6ac-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="ac6ac-114">สำหรับข้อมูลเพิ่มเติมให้ดูที่[การโอนการสมัครใช้งานไปยังผู้ใช้ในผู้เช่า AZURE AD รายอื่น](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ac6ac-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ac6ac-115">**เอกสารที่แนะนำ**</span><span class="sxs-lookup"><span data-stu-id="ac6ac-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="ac6ac-116">โอนความเป็นเจ้าของการเรียกเก็บเงินของการสมัครใช้งาน Azure ไปยังบัญชีผู้ใช้อื่น</span><span class="sxs-lookup"><span data-stu-id="ac6ac-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="ac6ac-117">เกี่ยวกับการโอนความเป็นเจ้าของการเรียกเก็บเงินสำหรับการสมัครใช้งาน Azure</span><span class="sxs-lookup"><span data-stu-id="ac6ac-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="ac6ac-118">การถ่ายโอน Visual Studio, Microsoft Partner Network (MPN) และชำระเงินตามที่คุณไปยังการสมัครใช้งาน Dev/ทดสอบ</span><span class="sxs-lookup"><span data-stu-id="ac6ac-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="ac6ac-119">คำถามที่ถามบ่อยเกี่ยวกับการโอนสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="ac6ac-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="ac6ac-120">การแก้ไขปัญหาการโอนความเป็นเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="ac6ac-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
