---
title: เพิ่มกลุ่มไปยังไซต์ SharePoint
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6ac4728c02471dd2640e0c516fee7cf5ebb12f54
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676408"
---
# <a name="add-a-group-to-a-sharepoint-site"></a><span data-ttu-id="6b1c0-102">เพิ่มกลุ่มไปยังไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b1c0-102">Add a group to a SharePoint site</span></span>

<span data-ttu-id="6b1c0-103">ไซต์ทีม SharePoint บางไซต์ (รวมถึงไซต์ที่สร้างใน Microsoft Teams) จะได้รับการจัดการโดยเจ้าของกลุ่มของ Office 365</span><span class="sxs-lookup"><span data-stu-id="6b1c0-103">Some SharePoint team sites (including those created in Microsoft Teams) are managed by Office 365 group owners.</span></span> <span data-ttu-id="6b1c0-104">ไซต์และเนื้อหา SharePoint ยังสามารถใช้ร่วมกับกลุ่ม Office 365 และกลุ่ม SharePoint ได้ด้วย</span><span class="sxs-lookup"><span data-stu-id="6b1c0-104">SharePoint sites and content can also be shared with Office 365 groups, and with SharePoint groups.</span></span> <span data-ttu-id="6b1c0-105">กลุ่ม SharePoint คือกลุ่มของผู้ใช้ที่ทุกคนมีสิทธิ์ชุดสิทธิ์เดียวกันกับไซต์และเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="6b1c0-105">A SharePoint group is a collection of users who all have the same set of permissions to sites and content.</span></span> <span data-ttu-id="6b1c0-106">สําหรับไซต์คลาสสิก เราขอแนะนําให้คุณใช้กลุ่มเพื่อกําหนดระดับสิทธิ์เดียวกันให้คนจํานวนมากในครั้งเดียวได้สะดวกแทนที่จะมอบหมายสิทธิ์ทีละคน</span><span class="sxs-lookup"><span data-stu-id="6b1c0-106">For classic sites, we recommend that you use groups to conveniently assign the same permission level to many people at once rather than assigning permissions one person at a time.</span></span>
  
<span data-ttu-id="6b1c0-107">จัดการสมาชิกกลุ่ม Office 365:</span><span class="sxs-lookup"><span data-stu-id="6b1c0-107">Manage Office 365 group members:</span></span>
  
1. <span data-ttu-id="6b1c0-108">ไปที่หน้า[กลุ่ม ใน ศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="6b1c0-108">Go to the [Groups page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="6b1c0-109">เลือกกลุ่มเพื่อดูเจ้าของและสมาชิก</span><span class="sxs-lookup"><span data-stu-id="6b1c0-109">Select a group to see its owners and members.</span></span> <span data-ttu-id="6b1c0-110">หากต้องการเพิ่มหรือนําบุคคลออก ให้คลิกลิงก์**แก้ไข**ในแถว**เจ้าของ**หรือ**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="6b1c0-110">To add or remove people, click the **Edit** link in the **Owners** or **Members** row.</span></span> 
    
<span data-ttu-id="6b1c0-111">แชร์ไซต์การสื่อสารกับกลุ่ม Office 365:</span><span class="sxs-lookup"><span data-stu-id="6b1c0-111">Share a communication site with an Office 365 group:</span></span>
  
1. <span data-ttu-id="6b1c0-112">ไปที่ไซต์ในเบราว์เซอร์แล้วคลิก**แชร์ไซต์**ที่ด้านขวาบน</span><span class="sxs-lookup"><span data-stu-id="6b1c0-112">Go to the site in a browser and click **Share site** in the upper right.</span></span> 
    
2. <span data-ttu-id="6b1c0-113">ป้อนชื่อกลุ่ม แล้วเลือกระดับสิทธิ์ (อ่าน แก้ไข หรือ ควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="6b1c0-113">Enter the group name, and then select the permission level (Read, Edit, or Full Control).</span></span>
    
<span data-ttu-id="6b1c0-114">สร้างกลุ่ม SharePoint เพื่อใช้กับไซต์แบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="6b1c0-114">Create a SharePoint group to use with a classic site:</span></span>
  
1. <span data-ttu-id="6b1c0-115">ไปที่เว็บไซต์ในเบราว์เซอร์และคลิกไอคอนการตั้งค่าที่มุมขวาบน</span><span class="sxs-lookup"><span data-stu-id="6b1c0-115">Go to the site in a browser and click the Settings icon in the upper right.</span></span>
    
2. <span data-ttu-id="6b1c0-116">คลิก**การตั้งค่าไซต์**จากนั้นภายใต้**ผู้ใช้และสิทธิ์**ให้คลิก**สิทธิ์ของไซต์**</span><span class="sxs-lookup"><span data-stu-id="6b1c0-116">Click **Site settings**, and then under **Users and Permissions**, click **Site permissions**.</span></span>
    
3. <span data-ttu-id="6b1c0-117">บนแท็บ สิทธิ ให้คลิก**สร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="6b1c0-117">On the Permissions tab, click **Create Group**.</span></span>
    
[<span data-ttu-id="6b1c0-118">เชื่อมต่อทีมไซต์แบบคลาสสิกกับกลุ่ม Office 365 ใหม่</span><span class="sxs-lookup"><span data-stu-id="6b1c0-118">Connect a classic team site to a new Office 365 group</span></span>](https://go.microsoft.com/fwlink/?linkid=2008654)
  
[<span data-ttu-id="6b1c0-119">เรียนรู้เพิ่มเติมเกี่ยวกับการทํางานกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b1c0-119">Learn more about working with SharePoint groups</span></span>](https://go.microsoft.com/fwlink/?linkid=874658)
  

