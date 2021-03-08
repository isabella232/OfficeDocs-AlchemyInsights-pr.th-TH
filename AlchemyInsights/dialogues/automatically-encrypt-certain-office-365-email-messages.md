---
title: เข้ารหัสลับบางข้อความอีเมล Office 365 โดยอัตโนมัติ
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527617"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="b2ad9-102">เข้ารหัสลับบางข้อความอีเมล Office 365 โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="b2ad9-103">คุณสามารถเข้ารหัสลับข้อความที่ผู้ใช้ส่งไปยังบุคคลหรือองค์กรภายนอกบางรายได้โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="b2ad9-104">เมื่อต้องการเลือกให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b2ad9-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="b2ad9-105">จากศูนย์ [การจัดการ Exchange](https://outlook.office365.com/ecp/)ให้เลือก **ล>จดหมายตาม** กฎ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="b2ad9-106">คลิกไอคอน **ใหม่ (+)** แล้วคลิก ใช้การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ **Office 365 กับ** ข้อความ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="b2ad9-107">ในชื่อ ให้ใส่ชื่อของกฎ เช่น เข้ารหัสลับข้อความที่ *ส่งไปยังDrToniRamos@gmail.com*</span><span class="sxs-lookup"><span data-stu-id="b2ad9-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="b2ad9-108">ใน **ใช้กฎนี้** ถ้า เลือก **>คือบุคคล** นี้</span><span class="sxs-lookup"><span data-stu-id="b2ad9-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="b2ad9-109">ในหน้าต่าง **เลือก** สมาชิก ให้เลือกชื่อของบุคคลที่คุณต้องการปรับใช้กฎการเข้ารหัสลับ **แล้วคลิก** เพิ่ม</span><span class="sxs-lookup"><span data-stu-id="b2ad9-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="b2ad9-110">เมื่อคุณเพิ่มผู้ใช้เสร็จแล้ว **ให้คลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="b2ad9-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="b2ad9-111">ถัดจากเขตข้อมูล **Do the following** ให้คลิก **เลือกหนึ่ง** รายการ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="b2ad9-112">ในเมนูดรอปดาวน์ของเทมเพลต **RMS** ให้เลือกเข้ารหัสลับ **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="b2ad9-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="b2ad9-113">(ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="b2ad9-114">แต่คุณสามารถเพิ่มได้)</span><span class="sxs-lookup"><span data-stu-id="b2ad9-114">But you can add it!)</span></span>
9. <span data-ttu-id="b2ad9-115">เลือกตัวเลือกใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างด้วยการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)</span><span class="sxs-lookup"><span data-stu-id="b2ad9-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="b2ad9-116">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b2ad9-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b2ad9-117">คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ</span><span class="sxs-lookup"><span data-stu-id="b2ad9-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="b2ad9-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="b2ad9-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

