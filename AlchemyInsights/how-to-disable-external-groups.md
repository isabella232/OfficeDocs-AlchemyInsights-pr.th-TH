---
title: วิธีการปิดการใช้งานของกลุ่มภายนอก
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899155"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="1a4d7-102">วิธีการปิดการใช้งานของกลุ่มภายนอก</span><span class="sxs-lookup"><span data-stu-id="1a4d7-102">How to disable External Groups</span></span>

<span data-ttu-id="1a4d7-p101">Yammer ส่งข้อความภายนอกใช้ขนส่งกฎการแลกเปลี่ยน (ETRs), ชุดของตัวควบคุมมาตรการเพื่อป้องกันไม่ให้ข้อมูลบริษัทถูกใช้ร่วมกัน เมื่อต้องการจำกัดผู้ใช้จากการสร้างกลุ่มภายนอก คุณจำเป็นต้องตั้งค่าคอนฟิกกฎการขนส่งอัตราแลกเปลี่ยน (ETR), และกำหนดค่า Yammer เพื่อใช้กฎในการขนส่งอัตราแลกเปลี่ยนเมื่อต้องการบล็อกการส่งข้อความภายนอก</span><span class="sxs-lookup"><span data-stu-id="1a4d7-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="1a4d7-105">หลังจากที่คุณได้สร้างกฎในศูนย์ดูแล Exchange แบบออนไลน์ ให้ทำตามขั้นตอนเหล่านี้เพื่อตั้งค่า ETR จะนำไปใช้ใน Yammer:</span><span class="sxs-lookup"><span data-stu-id="1a4d7-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="1a4d7-106">เข้าสู่ระบบ Yammer เป็นผู้ดูแลระบบผ่านการตรวจสอบ และการ**ดูแลศูนย์ Yammer**ไป C**เนื้อหา และความปลอดภัย\>ตั้งค่าความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="1a4d7-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="1a4d7-107">ภายใต้การ**ส่งข้อความภายนอก**เลือก**บังคับใช้กฎของคุณแลกเปลี่ยนออนไลน์แลกเปลี่ยนขนส่ง (ETRs) ใน Yammer**</span><span class="sxs-lookup"><span data-stu-id="1a4d7-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="1a4d7-108">เลือก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="1a4d7-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="1a4d7-109">สำหรับข้อมูลเพิ่มเติม ให้ดูที่[ควบคุมการส่งข้อความในเครือข่าย Yammer มีกฎการแลกเปลี่ยนการขนส่งภายนอก](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="1a4d7-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

