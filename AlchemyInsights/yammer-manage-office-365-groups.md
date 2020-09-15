---
title: 'Yammer-จัดการกลุ่ม Microsoft ๓๖๕ '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "995"
- "6000003"
ms.openlocfilehash: 543972a81a8958951e31d63a632283d07c06de4c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668906"
---
# <a name="manage-microsoft-365-groups-in-yammer"></a><span data-ttu-id="deb2b-102">จัดการกลุ่ม Microsoft ๓๖๕ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="deb2b-102">Manage Microsoft 365 Groups in Yammer</span></span>

<span data-ttu-id="deb2b-103">ต่อไปนี้เป็นคำตอบของปัญหาทั่วไปส่วนใหญ่เกี่ยวกับกลุ่ม Microsoft ๓๖๕ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="deb2b-103">Here are some answers to most common issues with Microsoft 365 Groups in Yammer.</span></span>

* <span data-ttu-id="deb2b-104">**กลุ่ม Microsoft ๓๖๕** เป็นพื้นที่ทำงานที่แชร์สำหรับอีเมลการสนทนาไฟล์และเหตุการณ์ที่สมาชิกกลุ่มสามารถทำงานร่วมกันได้</span><span class="sxs-lookup"><span data-stu-id="deb2b-104">**Microsoft 365 Groups** are a shared workspace for email, conversations, files, and events where group members can collaborate.</span></span> <span data-ttu-id="deb2b-105">เมื่อใช้ Yammer กลุ่ม Microsoft ๓๖๕จะมีข้อดีหลายประการกว่ากลุ่ม Yammer ที่ไม่ได้เชื่อมต่อ</span><span class="sxs-lookup"><span data-stu-id="deb2b-105">With Yammer, Microsoft 365 Groups have many advantages over non-connected Yammer groups.</span></span> <span data-ttu-id="deb2b-106">ตัวอย่างเช่นคุณสามารถสร้างและโฮสต์เหตุการณ์ live คืนค่ากลุ่มที่ถูกลบให้ใช้การเป็นสมาชิกของกลุ่มแบบไดนามิกที่เก็บถาวรอัตโนมัติและเข้าถึงทรัพยากรที่ใช้ร่วมกันเช่น Sharepoint, OneNote และโปรแกรมวางแผน</span><span class="sxs-lookup"><span data-stu-id="deb2b-106">For example, you can create and host live events, restore deleted groups, use dynamic group membership, auto archive, and access shared resources such as Sharepoint, OneNote, and Planner.</span></span>

* <span data-ttu-id="deb2b-107">คุณสามารถบอกได้ว่ากลุ่ม Yammer เชื่อมต่อกับกลุ่ม Microsoft ๓๖๕เมื่อคุณเห็นส่วน **ทรัพยากรของ Office ๓๖๕** (Sharepoint, OneNote, การวางแผน) ในการนำทางด้านขวาของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="deb2b-107">You can tell if a Yammer group is connected with Microsoft 365 Groups when you see the **Office 365 Resources** section (Sharepoint, OneNote, Planner) in the right navigation of the group.</span></span> <span data-ttu-id="deb2b-108">ถ้าทรัพยากรไม่พร้อมใช้งานให้ตรวจสอบสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="deb2b-108">If the resources are not available, check the following.</span></span>

  1. <span data-ttu-id="deb2b-109">เครือข่าย Yammer ต้องอยู่ใน1ผู้เช่า: 1 การกำหนดค่าเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="deb2b-109">The Yammer network must be in a 1 tenant:1 network configuration.</span></span> <span data-ttu-id="deb2b-110">เมื่อต้องการตรวจสอบว่าคุณอยู่ในการกำหนดค่า1:1 ให้ใช้ **เครื่องมือการโยกย้ายเครือข่าย** ตามที่อธิบายไว้ในการ [โยกย้ายเครือข่าย-รวมรวมเครือข่าย Yammer หลายเครือ](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)ข่าย</span><span class="sxs-lookup"><span data-stu-id="deb2b-110">to verify that you are in a 1:1 configuration, use the **Network Migration tool** as described in [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

  2. <span data-ttu-id="deb2b-111">เรียกดู **ผู้ดูแลระบบเครือข่ายการตั้งค่าความปลอดภัย**และตรวจสอบให้แน่ใจว่ามีการบังคับใช้ **ข้อมูลประจำตัวของ Office ๓๖๕** สำหรับผู้ใช้ Yammer</span><span class="sxs-lookup"><span data-stu-id="deb2b-111">Browse to **Network Admin, Security Setting**, and ensure that **Office 365 Identity** is enforced for Yammer users.</span></span>

<span data-ttu-id="deb2b-112">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกลุ่ม Microsoft ๓๖๕และ Yammer โปรดดูที่[กลุ่ม Yammer และ Microsoft ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="deb2b-112">For more information on Microsoft 365 Groups and Yammer, please see [Yammer and Microsoft 365 Groups](https://docs.microsoft.com/yammer/manage-yammer-groups/yammer-and-office-365-groups).</span></span> <span data-ttu-id="deb2b-113">สำหรับข้อมูลเกี่ยวกับการจัดการกลุ่มให้ดูที่ [จัดการกลุ่มใน Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span><span class="sxs-lookup"><span data-stu-id="deb2b-113">For information on managing a group, see [Manage a group in Yammer](https://support.office.com/article/Manage-a-group-in-Yammer-6e05c6d6-5548-4c88-89cd-e6757a514ef2)</span></span>
