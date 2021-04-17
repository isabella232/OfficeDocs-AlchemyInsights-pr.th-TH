---
title: 'Yammer - จัดการกลุ่ม Microsoft 365 '
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "995"
- "6000003"
ms.openlocfilehash: eb5959f74793ce146d326d2ddc32c359daecc3ba
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834102"
---
# <a name="manage-microsoft-365-groups-in-yammer"></a><span data-ttu-id="5992d-102">จัดการกลุ่ม Microsoft 365 ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="5992d-102">Manage Microsoft 365 Groups in Yammer</span></span>

<span data-ttu-id="5992d-103">ต่อไปนี้เป็นคําตอบของปัญหาทั่วไปส่วนใหญ่เกี่ยวกับกลุ่ม Microsoft 365 ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="5992d-103">Here are some answers to most common issues with Microsoft 365 Groups in Yammer.</span></span>

* <span data-ttu-id="5992d-104">**กลุ่ม Microsoft 365** เป็นพื้นที่การใช้ร่วมกันของอีเมล การสนทนา ไฟล์ และเหตุการณ์ที่สมาชิกกลุ่มสามารถร่วมกันได้</span><span class="sxs-lookup"><span data-stu-id="5992d-104">**Microsoft 365 Groups** are a shared workspace for email, conversations, files, and events where group members can collaborate.</span></span> <span data-ttu-id="5992d-105">ด้วย Yammer กลุ่ม Microsoft 365 มีข้อดีมากมายมากกว่ากลุ่ม Yammer ที่ไม่เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="5992d-105">With Yammer, Microsoft 365 Groups have many advantages over non-connected Yammer groups.</span></span> <span data-ttu-id="5992d-106">ตัวอย่างเช่น คุณสามารถสร้างและโฮสต์เหตุการณ์สด คืนค่ากลุ่มที่ถูกลบ ใช้การเป็นสมาชิกกลุ่มแบบไดนามิก การเก็บถาวรอัตโนมัติ และเข้าถึงแหล่งข้อมูลที่แชร์ เช่น Sharepoint, OneNote และ Planner</span><span class="sxs-lookup"><span data-stu-id="5992d-106">For example, you can create and host live events, restore deleted groups, use dynamic group membership, auto archive, and access shared resources such as Sharepoint, OneNote, and Planner.</span></span>

* <span data-ttu-id="5992d-107">คุณสามารถดูว่ากลุ่ม Yammer เชื่อมต่อกับกลุ่ม Microsoft 365 หรือไม่ เมื่อคุณเห็นส่วน แหล่งข้อมูล **Office 365** (Sharepoint, OneNote, Planner) ในการนําทางที่ถูกต้องของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="5992d-107">You can tell if a Yammer group is connected with Microsoft 365 Groups when you see the **Office 365 Resources** section (Sharepoint, OneNote, Planner) in the right navigation of the group.</span></span> <span data-ttu-id="5992d-108">ถ้าทรัพยากรไม่พร้อมใช้งาน ให้ตรวจสอบดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5992d-108">If the resources are not available, check the following.</span></span>

  1. <span data-ttu-id="5992d-109">เครือข่าย Yammer ต้องอยู่ในผู้เช่า 1:1 การกําหนดค่าเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="5992d-109">The Yammer network must be in a 1 tenant:1 network configuration.</span></span> <span data-ttu-id="5992d-110">เพื่อตรวจสอบว่าคุณอยู่ในการกําหนดค่า 1:1 ให้ใช้เครื่องมือ **การ** โยกย้ายเครือข่ายตามที่อธิบายไว้ในการโยกย้ายเครือข่าย [- รวมเครือข่าย Yammer หลาย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="5992d-110">to verify that you are in a 1:1 configuration, use the **Network Migration tool** as described in [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

  2. <span data-ttu-id="5992d-111">เรียกดู ผู้ดูแลระบบ **เครือข่าย การตั้งค่าความปลอดภัย และตรวจสอบ** ให้แน่ใจว่ามีการบังคับใช้ข้อมูลเฉพาะตัวของ Office **365** ให้กับผู้ใช้ Yammer</span><span class="sxs-lookup"><span data-stu-id="5992d-111">Browse to **Network Admin, Security Setting**, and ensure that **Office 365 Identity** is enforced for Yammer users.</span></span>

<span data-ttu-id="5992d-112">ดูข้อมูลเพิ่มเติมเกี่ยวกับกลุ่ม Microsoft 365 และ Yammer โปรดดู[กลุ่ม Yammer และ Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="5992d-112">For more information on Microsoft 365 Groups and Yammer, please see [Yammer and Microsoft 365 Groups](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups).</span></span> <span data-ttu-id="5992d-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span><span class="sxs-lookup"><span data-stu-id="5992d-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span></span>
