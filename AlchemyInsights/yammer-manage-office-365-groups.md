---
title: 'Yammer - จัดการกลุ่ม Office 365 '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "995"
- "6000003"
ms.openlocfilehash: 0257be866d6f6c654a28a4109ca7c9e6c34fc376
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715867"
---
# <a name="manage-office-365-groups-in-yammer"></a><span data-ttu-id="31d4a-102">จัดการกลุ่ม Office 365 ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="31d4a-102">Manage Office 365 groups in Yammer</span></span>

<span data-ttu-id="31d4a-103">ต่อไปนี้เป็นคําตอบสําหรับปัญหาทั่วไปเกี่ยวกับกลุ่ม Office 365 ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="31d4a-103">Here are some answers to most common issues with Office 365 groups in Yammer.</span></span>

* <span data-ttu-id="31d4a-104">**กลุ่ม Office 365**เป็นพื้นที่ทํางานที่ใช้ร่วมกันสําหรับอีเมล การสนทนา ไฟล์ และเหตุการณ์ที่สมาชิกกลุ่มสามารถทํางานร่วมกันได้</span><span class="sxs-lookup"><span data-stu-id="31d4a-104">**Office 365 Groups** are a shared workspace for email, conversations, files, and events where group members can collaborate.</span></span> <span data-ttu-id="31d4a-105">กลุ่ม Office 365 มีข้อดีมากมายเหนือกลุ่ม Yammer ที่ไม่ได้เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="31d4a-105">With Yammer, Office 365 groups have many advantages over non-connected Yammer groups.</span></span> <span data-ttu-id="31d4a-106">ตัวอย่างเช่น คุณสามารถสร้างและโฮสต์เหตุการณ์สด เรียกคืนกลุ่มที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="31d4a-106">For example, you can create and host live events, restore deleted groups, use dynamic group membership, auto archive, and access shared resources such as Sharepoint, OneNote, and Planner.</span></span>

* <span data-ttu-id="31d4a-107">คุณสามารถบอกได้ว่า กลุ่ม Yammer เชื่อมต่อกับกลุ่ม Office 365 เมื่อคุณเห็นส่วน**ทรัพยากร Office 365** (Sharepoint, OneNote, Planner) ในการนําทางด้านขวาของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="31d4a-107">You can tell if a Yammer group is connected with Office 365 groups when you see the **Office 365 Resources** section (Sharepoint, OneNote, Planner) in the right navigation of the group.</span></span> <span data-ttu-id="31d4a-108">ถ้าทรัพยากรไม่พร้อมใช้งาน ให้ตรวจสอบต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="31d4a-108">If the resources are not available, check the following.</span></span>

  1. <span data-ttu-id="31d4a-109">เครือข่าย Yammer ต้องอยู่ในการกําหนดค่าเครือข่าย 1 ผู้เช่า:1</span><span class="sxs-lookup"><span data-stu-id="31d4a-109">The Yammer network must be in a 1 tenant:1 network configuration.</span></span> <span data-ttu-id="31d4a-110">เพื่อตรวจสอบว่าคุณอยู่ในการกําหนดค่าแบบ 1:1 ให้ใช้**เครื่องมือการโยกย้ายเครือข่าย**ตามที่อธิบายไว้ใน[การโยกย้ายเครือข่าย - รวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="31d4a-110">to verify that you are in a 1:1 configuration, use the **Network Migration tool** as described in [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

  2. <span data-ttu-id="31d4a-111">เรียกดู**ผู้ดูแลระบบเครือข่าย การตั้งค่าความปลอดภัย**และตรวจสอบให้แน่ใจว่าข้อมูลประจําตัว**Office 365**ถูกบังคับใช้สําหรับผู้ใช้ Yammer</span><span class="sxs-lookup"><span data-stu-id="31d4a-111">Browse to **Network Admin, Security Setting**, and ensure that **Office 365 Identity** is enforced for Yammer users.</span></span>

<span data-ttu-id="31d4a-112">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่ม Office 365 และ Yammer โปรดดู[กลุ่ม Yammer และ 365 สํานักงาน](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="31d4a-112">For more information on Office 365 groups and Yammer, please see [Yammer and office 365 Groups](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups).</span></span> <span data-ttu-id="31d4a-113">สําหรับข้อมูลเกี่ยวกับการจัดการกลุ่ม ให้ดูที่[จัดการกลุ่มใน Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span><span class="sxs-lookup"><span data-stu-id="31d4a-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span></span>
