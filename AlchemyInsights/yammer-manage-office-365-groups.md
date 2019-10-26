---
title: 'Yammer-จัดการ Office ๓๖๕กลุ่ม '
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
ms.openlocfilehash: 9c2742b715064d55d9525860f78c530294f90999
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36530982"
---
# <a name="manage-office-365-groups-in-yammer"></a><span data-ttu-id="1a2d7-102">จัดการกลุ่ม Office ๓๖๕ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="1a2d7-102">Manage Office 365 groups in Yammer</span></span>

<span data-ttu-id="1a2d7-103">ต่อไปนี้เป็นคำตอบบางส่วนสำหรับปัญหาทั่วไปเกี่ยวกับ Office ๓๖๕กลุ่มใน Yammer</span><span class="sxs-lookup"><span data-stu-id="1a2d7-103">Here are some answers to most common issues with Office 365 groups in Yammer.</span></span>

* <span data-ttu-id="1a2d7-104">**Office ๓๖๕กลุ่ม**เป็นพื้นที่ทำงานที่ใช้ร่วมกันสำหรับการส่งเมลการสนทนาไฟล์และเหตุการณ์ที่สมาชิกกลุ่มสามารถทำงานร่วมกับคุณได้</span><span class="sxs-lookup"><span data-stu-id="1a2d7-104">**Office 365 Groups** are a shared workspace for email, conversations, files, and events where group members can collaborate.</span></span> <span data-ttu-id="1a2d7-105">ด้วย Yammer กลุ่ม Office ๓๖๕มีข้อดีมากกว่ากลุ่ม Yammer ที่ไม่มีการเชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="1a2d7-105">With Yammer, Office 365 groups have many advantages over non-connected Yammer groups.</span></span> <span data-ttu-id="1a2d7-106">ตัวอย่างเช่นคุณสามารถสร้างและโฮสต์เหตุการณ์สดกู้คืนกลุ่มที่ถูกลบให้ใช้สมาชิกกลุ่มแบบไดนามิกที่เก็บถาวรอัตโนมัติและเข้าถึงทรัพยากรที่ใช้ร่วมกันเช่น Sharepoint, OneNote และโปรแกรมวางแผน</span><span class="sxs-lookup"><span data-stu-id="1a2d7-106">For example, you can create and host live events, restore deleted groups, use dynamic group membership, auto archive, and access shared resources such as Sharepoint, OneNote, and Planner.</span></span>

* <span data-ttu-id="1a2d7-107">คุณสามารถบอกได้ว่ากลุ่ม Yammer เชื่อมต่อกับกลุ่ม Office ๓๖๕เมื่อคุณเห็นส่วน**ทรัพยากร office ๓๖๕**(Sharepoint, OneNote, โปรแกรมวางแผน) ในการนำทางที่ถูกต้องของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="1a2d7-107">You can tell if a Yammer group is connected with Office 365 groups when you see the **Office 365 Resources** section (Sharepoint, OneNote, Planner) in the right navigation of the group.</span></span> <span data-ttu-id="1a2d7-108">ถ้าไม่มีทรัพยากรให้ตรวจสอบดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="1a2d7-108">If the resources are not available, check the following.</span></span>

  1. <span data-ttu-id="1a2d7-109">เครือข่าย Yammer ต้องอยู่ในผู้เช่า 1: 1 การกำหนดค่าเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="1a2d7-109">The Yammer network must be in a 1 tenant:1 network configuration.</span></span> <span data-ttu-id="1a2d7-110">เพื่อตรวจสอบว่าคุณอยู่ในการตั้งค่าคอนฟิก1:1 ใช้**เครื่องมือการโยกย้ายเครือข่าย**ตามที่อธิบายไว้ในการ[โยกย้ายเครือข่าย-รวมหลายเครือข่าย Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="1a2d7-110">to verify that you are in a 1:1 configuration, use the **Network Migration tool** as described in [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

  2. <span data-ttu-id="1a2d7-111">เรียกดูไปยังผู้**ดูแลเครือข่ายการตั้งค่าความปลอดภัย**และตรวจสอบให้แน่ใจว่ามีการบังคับใช้**ข้อมูลเฉพาะตัวของ Office ๓๖๕**สำหรับผู้ทำงาน Yammer</span><span class="sxs-lookup"><span data-stu-id="1a2d7-111">Browse to **Network Admin, Security Setting**, and ensure that **Office 365 Identity** is enforced for Yammer users.</span></span>

<span data-ttu-id="1a2d7-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ Office ๓๖๕กลุ่มและ Yammer โปรดดูที่[Yammer และ Office ๓๖๕กลุ่ม](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups?redirectSourcePath=%252fen-us%252farticle%252fYammer-and-Office-365-Groups-d8c239dc-a48b-47ab-b85e-6b4b8191a869)</span><span class="sxs-lookup"><span data-stu-id="1a2d7-112">For more information on Office 365 groups and Yammer, please see [Yammer and office 365 Groups](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups?redirectSourcePath=%252fen-us%252farticle%252fYammer-and-Office-365-Groups-d8c239dc-a48b-47ab-b85e-6b4b8191a869).</span></span> <span data-ttu-id="1a2d7-113">สำหรับข้อมูลเกี่ยวกับการจัดการกลุ่มให้ดูที่[จัดการกลุ่มใน Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span><span class="sxs-lookup"><span data-stu-id="1a2d7-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span></span>
