---
title: วิธีการปิดใช้งานกลุ่มภายนอก
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704147"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="cd0c1-102">วิธีการปิดใช้งานกลุ่มภายนอก</span><span class="sxs-lookup"><span data-stu-id="cd0c1-102">How to disable External Groups</span></span>

<span data-ttu-id="cd0c1-103">การส่งข้อความภายนอกของ Yammer ใช้กฎการขนส่ง Exchange (Etr) ชุดของตัวควบคุมเชิงรุกเพื่อป้องกันไม่ให้มีการแชร์ข้อมูลของบริษัท</span><span class="sxs-lookup"><span data-stu-id="cd0c1-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="cd0c1-104">เมื่อต้องการจำกัดผู้ใช้จากการสร้างกลุ่มภายนอกคุณจำเป็นต้องกำหนดค่ากฎการขนส่ง Exchange (ETR) แล้วกำหนดค่า Yammer ให้ใช้กฎการขนส่ง Exchange เพื่อบล็อกการส่งข้อความภายนอก</span><span class="sxs-lookup"><span data-stu-id="cd0c1-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="cd0c1-105">เมื่อคุณสร้างกฎในศูนย์การจัดการ Exchange Online แล้วให้ทำตามขั้นตอนต่อไปนี้เพื่อตั้งค่า ETR เพื่อนำไปใช้ใน Yammer:</span><span class="sxs-lookup"><span data-stu-id="cd0c1-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="cd0c1-106">เข้าสู่ระบบ Yammer เป็นผู้ดูแลระบบที่ผ่านการตรวจสอบและใน**ศูนย์การจัดการ Yammer**ให้ไปที่การ\*\* \> ตั้งค่าการรักษาความปลอดภัยของเนื้อหาและการรักษาความปลอดภัย\*\*ของ C</span><span class="sxs-lookup"><span data-stu-id="cd0c1-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="cd0c1-107">ภายใต้การ **ส่งข้อความภายนอก**ให้เลือก **บังคับใช้กฎการขนส่ง exchange Online exchange ของคุณ (Etr) ใน Yammer**</span><span class="sxs-lookup"><span data-stu-id="cd0c1-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="cd0c1-108">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="cd0c1-108">Choose **Save**.</span></span>

<span data-ttu-id="cd0c1-109">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ปิดใช้งานการส่งข้อความภายนอกในเครือข่าย Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)</span><span class="sxs-lookup"><span data-stu-id="cd0c1-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  