---
title: การเพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: c2bb1ce655e994054278927dfe346c0decd09f19
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36495230"
---
# <a name="add-a-group-to-a-sharepoint-site"></a><span data-ttu-id="910ca-102">การเพิ่มกลุ่มลงในไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="910ca-102">Add a group to a SharePoint site</span></span>

<span data-ttu-id="910ca-103">บางไซต์ทีม SharePoint (รวมทั้งที่สร้างขึ้นใน Microsoft Teams) จะถูกจัดการโดยเจ้าของกลุ่ม Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="910ca-103">Some SharePoint team sites (including those created in Microsoft Teams) are managed by Office 365 group owners.</span></span> <span data-ttu-id="910ca-104">ไซต์ SharePoint และเนื้อหายังสามารถใช้ร่วมกันกับกลุ่ม Office ๓๖๕และกับกลุ่ม SharePoint ได้ด้วย</span><span class="sxs-lookup"><span data-stu-id="910ca-104">SharePoint sites and content can also be shared with Office 365 groups, and with SharePoint groups.</span></span> <span data-ttu-id="910ca-105">กลุ่ม SharePoint คือคอลเลกชันของผู้ใช้ที่ทุกคนมีชุดของสิทธิ์เดียวกันกับไซต์และเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="910ca-105">A SharePoint group is a collection of users who all have the same set of permissions to sites and content.</span></span> <span data-ttu-id="910ca-106">สำหรับเว็บไซต์คลาสสิกเราขอแนะนำให้คุณใช้กลุ่มเพื่อมอบหมายระดับสิทธิการได้รับอนุญาตเดียวกันให้กับผู้คนจำนวนมากในครั้งเดียวแทนที่จะกำหนดสิทธิ์หนึ่งคนในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="910ca-106">For classic sites, we recommend that you use groups to conveniently assign the same permission level to many people at once rather than assigning permissions one person at a time.</span></span>
  
<span data-ttu-id="910ca-107">จัดการสมาชิกของกลุ่ม Office ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="910ca-107">Manage Office 365 group members:</span></span>
  
1. <span data-ttu-id="910ca-108">ไปที่[หน้ากลุ่มในศูนย์ดูแลของ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="910ca-108">Go to the [Groups page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="910ca-109">เลือกกลุ่มเพื่อดูเจ้าของและสมาชิก</span><span class="sxs-lookup"><span data-stu-id="910ca-109">Select a group to see its owners and members.</span></span> <span data-ttu-id="910ca-110">หากต้องการเพิ่มหรือนำผู้คนออกให้คลิกลิงก์**แก้ไข**ใน**เจ้าของ**หรือแถว**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="910ca-110">To add or remove people, click the **Edit** link in the **Owners** or **Members** row.</span></span> 
    
<span data-ttu-id="910ca-111">ใช้ไซต์การสื่อสารร่วมกับกลุ่ม Office ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="910ca-111">Share a communication site with an Office 365 group:</span></span>
  
1. <span data-ttu-id="910ca-112">ไปที่เว็บไซต์ในเบราว์เซอร์แล้วคลิก "**แชร์เว็บไซต์**" ที่ด้านขวาบน</span><span class="sxs-lookup"><span data-stu-id="910ca-112">Go to the site in a browser and click **Share site** in the upper right.</span></span> 
    
2. <span data-ttu-id="910ca-113">ป้อนชื่อกลุ่มแล้วเลือกระดับสิทธิ์ (อ่านแก้ไขหรือควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="910ca-113">Enter the group name, and then select the permission level (Read, Edit, or Full Control).</span></span>
    
<span data-ttu-id="910ca-114">สร้างกลุ่ม SharePoint ที่จะใช้กับไซต์คลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="910ca-114">Create a SharePoint group to use with a classic site:</span></span>
  
1. <span data-ttu-id="910ca-115">ไปที่เว็บไซต์ในเบราว์เซอร์แล้วคลิกไอคอนการตั้งค่าที่ด้านบนขวา</span><span class="sxs-lookup"><span data-stu-id="910ca-115">Go to the site in a browser and click the Settings icon in the upper right.</span></span>
    
2. <span data-ttu-id="910ca-116">คลิกการ**ตั้งค่าไซต์**จากนั้นภายใต้**ผู้ใช้และสิทธิ์**คลิ**กสิทธิ์ของไซต์**</span><span class="sxs-lookup"><span data-stu-id="910ca-116">Click **Site settings**, and then under **Users and Permissions**, click **Site permissions**.</span></span>
    
3. <span data-ttu-id="910ca-117">บนแท็บสิทธิ์คลิ**กสร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="910ca-117">On the Permissions tab, click **Create Group**.</span></span>
    
[<span data-ttu-id="910ca-118">เชื่อมต่อไซต์ทีมคลาสสิกกับกลุ่ม Office ๓๖๕ใหม่</span><span class="sxs-lookup"><span data-stu-id="910ca-118">Connect a classic team site to a new Office 365 group</span></span>](https://go.microsoft.com/fwlink/?linkid=2008654)
  
[<span data-ttu-id="910ca-119">เรียนรู้เพิ่มเติมเกี่ยวกับการทำงานกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="910ca-119">Learn more about working with SharePoint groups</span></span>](https://go.microsoft.com/fwlink/?linkid=874658)
  

