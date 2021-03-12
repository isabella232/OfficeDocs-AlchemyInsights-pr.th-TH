---
title: เข้ารหัสลับข้อความอีเมล Office 365 ที่ถูกส่งไปยังบางโดเมนโดยอัตโนมัติ
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749298"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="1172c-102">เข้ารหัสลับข้อความอีเมล Office 365 ที่ถูกส่งไปยังบางโดเมนโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1172c-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="1172c-103">จากศูนย์ [การจัดการ Exchange](https://outlook.office365.com/ecp/)ให้เลือก **ล>จดหมายตาม** กฎ</span><span class="sxs-lookup"><span data-stu-id="1172c-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="1172c-104">คลิกไอคอน **ใหม่ (+)** แล้วคลิก ใช้การเข้ารหัสลับข้อความและการป้องกันสิทธิ์ของ **Office 365 กับ** ข้อความ</span><span class="sxs-lookup"><span data-stu-id="1172c-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="1172c-105">ในชื่อ ให้ใส่ชื่อของกฎ เช่น เข้ารหัสข้อความที่ *ส่งไปยังcontoso.com*</span><span class="sxs-lookup"><span data-stu-id="1172c-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="1172c-106">ใน **ปรับใช้กฎนี้** ถ้า เลือก **>โดเมนคือ**</span><span class="sxs-lookup"><span data-stu-id="1172c-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="1172c-107">ใส่ชื่อของโดเมน เช่น contoso.com </span><span class="sxs-lookup"><span data-stu-id="1172c-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="1172c-108">คลิก **ไอคอน เพิ่ม (+)** **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="1172c-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="1172c-109">ถัดจากเขตข้อมูล **Do the following** ให้คลิก **เลือกหนึ่ง** รายการ</span><span class="sxs-lookup"><span data-stu-id="1172c-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="1172c-110">ในเมนูดรอปดาวน์ของเทมเพลต **RMS** **ให้เลือก** เข้ารหัสลับ **แล้วคลิก** ตกลง</span><span class="sxs-lookup"><span data-stu-id="1172c-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="1172c-111">(ถ้าคุณไม่เห็นตัวเลือกนี้ หมายความว่าแผนของคุณไม่มีการเข้ารหัสลับอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="1172c-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="1172c-112">แต่คุณสามารถเพิ่มได้)</span><span class="sxs-lookup"><span data-stu-id="1172c-112">But you can add it!)</span></span>
9. <span data-ttu-id="1172c-113">เลือกตัวเลือกใดก็ได้ (จากรายการตัวเลือกเพิ่มเติมที่คุณสามารถเลือกได้ณจุดนี้ โดยสามารถเลือกได้หลายอย่างด้วยการตั้งค่าเริ่มต้นเพื่อความเรียบง่าย)</span><span class="sxs-lookup"><span data-stu-id="1172c-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="1172c-114">คลิก **บันทึก**</span><span class="sxs-lookup"><span data-stu-id="1172c-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1172c-115">คุณสามารถกลับมาและแก้ไขกฎนี้ในภายหลังได้เสมอ</span><span class="sxs-lookup"><span data-stu-id="1172c-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="1172c-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="1172c-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>