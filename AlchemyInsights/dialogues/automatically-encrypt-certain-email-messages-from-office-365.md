---
title: เข้ารหัสลับบางข้อความอีเมลจาก Office 365 โดยอัตโนมัติ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527625"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="85c3b-102">เข้ารหัสลับบางข้อความอีเมลจาก Office 365 โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="85c3b-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="85c3b-103">จากศูนย์ [การจัดการ Exchange](https://outlook.office365.com/ecp/)ให้เลือก **ล>จดหมายตาม** กฎ</span><span class="sxs-lookup"><span data-stu-id="85c3b-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="85c3b-104">คลิกไอคอน **ใหม่ (+)** แล้วคลิก ใช้การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ **Office 365 กับ** ข้อความ</span><span class="sxs-lookup"><span data-stu-id="85c3b-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="85c3b-105">ในชื่อ ให้ใส่ชื่อของกฎ เช่น *เข้ารหัสลับข้อความ* ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="85c3b-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="85c3b-106">ใน **ปรับใช้กฎนี้ ให้เลือก** **[ใช้กับข้อความทั้งหมด]**</span><span class="sxs-lookup"><span data-stu-id="85c3b-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="85c3b-107">ถัดจากเขตข้อมูล **Do the following** ให้คลิก **เลือกหนึ่ง** รายการ</span><span class="sxs-lookup"><span data-stu-id="85c3b-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="85c3b-108">ในเมนูดรอปดาวน์ของเทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="85c3b-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="85c3b-109">(ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="85c3b-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="85c3b-110">แต่คุณสามารถเพิ่มได้)</span><span class="sxs-lookup"><span data-stu-id="85c3b-110">But you can add it!)</span></span>
7. <span data-ttu-id="85c3b-111">เลือกกล่องกา **เครื่องหมาย ตรวจสอบกฎนี้ด้วย** ระดับความรุนแรง แล้วเลือกระดับที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="85c3b-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="85c3b-112">ถ้าบริษัทของคุณมีข้อผูกมัดสัญญาที่จะส่งอีเมลทั้งหมดที่เข้ารหัสลับ ฉันขอแนะนนะให้ตั้งค่า **ระดับเป็น** สูง</span><span class="sxs-lookup"><span data-stu-id="85c3b-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="85c3b-113">ภายใต้ **เลือกตัวแบบของกฎ** นี้ **ให้คลิก** บังคับใช้</span><span class="sxs-lookup"><span data-stu-id="85c3b-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="85c3b-114">เลือกตัวเลือกใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างด้วยการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)</span><span class="sxs-lookup"><span data-stu-id="85c3b-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="85c3b-115">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="85c3b-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="85c3b-116">คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ</span><span class="sxs-lookup"><span data-stu-id="85c3b-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="85c3b-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="85c3b-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

