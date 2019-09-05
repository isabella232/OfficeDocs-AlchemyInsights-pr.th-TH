---
title: วิธีการปิดใช้งานกลุ่มภายนอก
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739512"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2ed87-102">วิธีการปิดใช้งานกลุ่มภายนอก</span><span class="sxs-lookup"><span data-stu-id="2ed87-102">How to disable External Groups</span></span>

<span data-ttu-id="2ed87-103">การส่งข้อความภายนอก Yammer ใช้กฎการขนส่งการแลกเปลี่ยน (ETRs), ชุดของตัวควบคุมเชิงรุกเพื่อป้องกันไม่ให้ข้อมูลของบริษัทถูกใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="2ed87-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2ed87-104">เพื่อจำกัดผู้ใช้จากการสร้างกลุ่มภายนอกคุณจำเป็นต้องกำหนดค่ากฎการขนส่งอัตราแลกเปลี่ยน (ETR), และตั้งค่าคอนฟิก Yammer เพื่อใช้กฎการขนส่งอัตราแลกเปลี่ยนเพื่อบล็อกการส่งข้อความภายนอก</span><span class="sxs-lookup"><span data-stu-id="2ed87-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="2ed87-105">เมื่อคุณได้สร้างกฎในศูนย์กลางการดูแล Exchange แบบออนไลน์ให้ทำตามขั้นตอนเหล่านี้เพื่อตั้งค่า ETR เพื่อใช้ใน Yammer:</span><span class="sxs-lookup"><span data-stu-id="2ed87-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2ed87-106">เข้าสู่ระบบ Yammer เป็นผู้ดูแลที่ได้ตรวจสอบแล้วและใน**ศูนย์ดูแล Yammer**ไปที่**การตั้งค่า\>ความปลอดภัยของเนื้อหา C และความ**ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="2ed87-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="2ed87-107">ภายใต้การ**ส่งข้อความภายนอก**เลือก**บังคับใช้กฎการขนส่ง exchange แบบออนไลน์ของอัตราแลกเปลี่ยนของคุณ (etrs) ใน Yammer**</span><span class="sxs-lookup"><span data-stu-id="2ed87-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="2ed87-108">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="2ed87-108">Choose **Save**.</span></span>

<span data-ttu-id="2ed87-109">สำหรับข้อมูลเพิ่มเติมโปรดดูที่[ปิดใช้งานการส่งข้อความภายนอกในเครือข่าย Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)</span><span class="sxs-lookup"><span data-stu-id="2ed87-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  