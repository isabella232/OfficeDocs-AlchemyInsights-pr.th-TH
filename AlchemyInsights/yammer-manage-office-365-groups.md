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
ms.openlocfilehash: 9c2742b715064d55d9525860f78c530294f90999
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530982"
---
# <a name="manage-office-365-groups-in-yammer"></a><span data-ttu-id="5e43d-102">จัดการกลุ่ม Office 365 ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="5e43d-102">Manage Office 365 groups in Yammer</span></span>

<span data-ttu-id="5e43d-103">ต่อไปนี้เป็นคำตอบสำหรับปัญหาทั่วไปเกี่ยวกับกลุ่ม Office 365 ใน Yammer บางคำ</span><span class="sxs-lookup"><span data-stu-id="5e43d-103">Here are some answers to most common issues with Office 365 groups in Yammer.</span></span>

* <span data-ttu-id="5e43d-104">**Office 365 กลุ่ม**งานที่ใช้ร่วมกันพื้นที่ทำงานสำหรับอีเมล การสนทนา แฟ้ม และเหตุการณ์ที่สมาชิกของกลุ่มสามารถทำงานร่วมอยู่</span><span class="sxs-lookup"><span data-stu-id="5e43d-104">**Office 365 Groups** are a shared workspace for email, conversations, files, and events where group members can collaborate.</span></span> <span data-ttu-id="5e43d-105">Yammer ช่วย กลุ่ม Office 365 มีข้อดีหลายประการที่ไม่เกี่ยวข้องกับกลุ่ม Yammer</span><span class="sxs-lookup"><span data-stu-id="5e43d-105">With Yammer, Office 365 groups have many advantages over non-connected Yammer groups.</span></span> <span data-ttu-id="5e43d-106">ตัวอย่างเช่น คุณสามารถสร้าง และโฮสต์ live เหตุการณ์ กลุ่มที่ถูกลบไปแล้วคืนค่า ใช้สมาชิกกลุ่มแบบไดนามิก เก็บถาวรอัตโนมัติ และเข้าถึงทรัพยากรที่ใช้ร่วมกันเช่น Sharepoint, OneNote วางแผน และ</span><span class="sxs-lookup"><span data-stu-id="5e43d-106">For example, you can create and host live events, restore deleted groups, use dynamic group membership, auto archive, and access shared resources such as Sharepoint, OneNote, and Planner.</span></span>

* <span data-ttu-id="5e43d-107">คุณสามารถบอกได้ว่า กลุ่ม Yammer เชื่อมต่อกับกลุ่ม Office 365 เมื่อคุณดู**Office 365 ทรัพยากร**(Sharepoint, OneNote วางแผน) ในการนำทางด้านขวาของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="5e43d-107">You can tell if a Yammer group is connected with Office 365 groups when you see the **Office 365 Resources** section (Sharepoint, OneNote, Planner) in the right navigation of the group.</span></span> <span data-ttu-id="5e43d-108">ถ้าทรัพยากรไม่พร้อมใช้งาน ตรวจสอบต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5e43d-108">If the resources are not available, check the following.</span></span>

  1. <span data-ttu-id="5e43d-109">เครือข่าย Yammer ต้องอยู่ในการกำหนดค่าเครือข่ายผู้เช่า: 1 1</span><span class="sxs-lookup"><span data-stu-id="5e43d-109">The Yammer network must be in a 1 tenant:1 network configuration.</span></span> <span data-ttu-id="5e43d-110">เมื่อต้องการตรวจสอบว่า คุณอยู่ในการตั้งค่าคอนฟิกเป็น 1:1 ใช้**เครื่องมือการโยกย้ายเครือข่าย**ตามที่อธิบายไว้ใน[เครือข่ายโยกย้าย - รวมหลายเครือข่าย Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="5e43d-110">to verify that you are in a 1:1 configuration, use the **Network Migration tool** as described in [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

  2. <span data-ttu-id="5e43d-111">เรียกดู**ผู้ดูแลเครือข่าย การตั้งค่าการรักษาความปลอดภัย**และให้แน่ใจว่า**Office 365 Identity**บังคับใช้สำหรับผู้ใช้ Yammer</span><span class="sxs-lookup"><span data-stu-id="5e43d-111">Browse to **Network Admin, Security Setting**, and ensure that **Office 365 Identity** is enforced for Yammer users.</span></span>

<span data-ttu-id="5e43d-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่ม Office 365 และ Yammer โปรดดู[Yammer และ office 365 กลุ่ม](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups?redirectSourcePath=%252fen-us%252farticle%252fYammer-and-Office-365-Groups-d8c239dc-a48b-47ab-b85e-6b4b8191a869)</span><span class="sxs-lookup"><span data-stu-id="5e43d-112">For more information on Office 365 groups and Yammer, please see [Yammer and office 365 Groups](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups?redirectSourcePath=%252fen-us%252farticle%252fYammer-and-Office-365-Groups-d8c239dc-a48b-47ab-b85e-6b4b8191a869).</span></span> <span data-ttu-id="5e43d-113">สำหรับข้อมูลเกี่ยวกับการจัดการกลุ่ม ดู[จัดการกลุ่มใน Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span><span class="sxs-lookup"><span data-stu-id="5e43d-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span></span>
