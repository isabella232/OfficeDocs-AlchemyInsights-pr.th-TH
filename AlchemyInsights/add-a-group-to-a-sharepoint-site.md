---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
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
ms.openlocfilehash: 2050d2affabbe15521bcfcbee5ea5651b61770a7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581286"
---
# <a name="add-a-group-to-a-sharepoint-site"></a><span data-ttu-id="deab3-102">เพิ่มกลุ่มลงในไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="deab3-102">Add a group to a SharePoint site</span></span>

<span data-ttu-id="deab3-103">ไซต์ทีมของ SharePoint บางไซต์ (รวมถึงไซต์ที่สร้างขึ้นใน Microsoft Teams) จะได้รับการจัดการโดยเจ้าของกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="deab3-103">Some SharePoint team sites (including those created in Microsoft Teams) are managed by Microsoft 365 group owners.</span></span> <span data-ttu-id="deab3-104">ไซต์และเนื้อหา SharePoint ยังสามารถใช้ร่วมกับกลุ่ม Microsoft 365 และกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="deab3-104">SharePoint sites and content can also be shared with Microsoft 365 groups, and with SharePoint groups.</span></span> <span data-ttu-id="deab3-105">กลุ่ม SharePoint คือกลุ่มผู้ใช้ที่มีสิทธิ์ในไซต์และเนื้อหาชุดเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="deab3-105">A SharePoint group is a collection of users who all have the same set of permissions to sites and content.</span></span> <span data-ttu-id="deab3-106">สําหรับไซต์คลาสสิก เราขอแนะนําให้คุณใช้กลุ่มเพื่อกําหนดระดับสิทธิ์เดียวกันให้กับบุคคลจํานวนมากในคราวเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="deab3-106">For classic sites, we recommend that you use groups to conveniently assign the same permission level to many people at once rather than assigning permissions one person at a time.</span></span>
  
<span data-ttu-id="deab3-107">จัดการสมาชิกกลุ่ม Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="deab3-107">Manage Microsoft 365 group members:</span></span>
  
1. <span data-ttu-id="deab3-108">ไปที่หน้า[กลุ่ม ในศูนย์การจัดการ Microsoft 365](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="deab3-108">Go to the [Groups page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="deab3-109">เลือกกลุ่มเพื่อดูเจ้าของและสมาชิก</span><span class="sxs-lookup"><span data-stu-id="deab3-109">Select a group to see its owners and members.</span></span> <span data-ttu-id="deab3-110">เมื่อต้องการเพิ่มหรือเอาบุคคลออก ให้คลิกลิงก์**แก้ไข**ในแถว**เจ้าของ**หรือ**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="deab3-110">To add or remove people, click the **Edit** link in the **Owners** or **Members** row.</span></span> 
    
<span data-ttu-id="deab3-111">แชร์ไซต์การสื่อสารกับกลุ่ม Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="deab3-111">Share a communication site with a Microsoft 365 group:</span></span>
  
1. <span data-ttu-id="deab3-112">ไปที่ไซต์ในเบราว์เซอร์ แล้วคลิก**แชร์ไซต์**ที่ด้านขวาบน</span><span class="sxs-lookup"><span data-stu-id="deab3-112">Go to the site in a browser and click **Share site** in the upper right.</span></span> 
    
2. <span data-ttu-id="deab3-113">ป้อนชื่อกลุ่ม แล้วเลือกระดับสิทธิ์ (อ่าน แก้ไข หรือควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="deab3-113">Enter the group name, and then select the permission level (Read, Edit, or Full Control).</span></span>
    
<span data-ttu-id="deab3-114">สร้างกลุ่ม SharePoint เพื่อใช้กับไซต์แบบคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="deab3-114">Create a SharePoint group to use with a classic site:</span></span>
  
1. <span data-ttu-id="deab3-115">ไปที่ไซต์ในเบราว์เซอร์ แล้วคลิกไอคอน การตั้งค่า ที่มุมขวาบน</span><span class="sxs-lookup"><span data-stu-id="deab3-115">Go to the site in a browser and click the Settings icon in the upper right.</span></span>
    
2. <span data-ttu-id="deab3-116">คลิก**การตั้งค่าไซต์**จากนั้นภายใต้**ผู้ใช้และสิทธิ์**ให้คลิก**สิทธิ์ของไซต์**</span><span class="sxs-lookup"><span data-stu-id="deab3-116">Click **Site settings**, and then under **Users and Permissions**, click **Site permissions**.</span></span>
    
3. <span data-ttu-id="deab3-117">บนแท็บ สิทธิ์ ให้คลิก**สร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="deab3-117">On the Permissions tab, click **Create Group**.</span></span>
    
[<span data-ttu-id="deab3-118">เชื่อมต่อไซต์ทีมคลาสสิกกับกลุ่ม Microsoft 365 ใหม่</span><span class="sxs-lookup"><span data-stu-id="deab3-118">Connect a classic team site to a new Microsoft 365 group</span></span>](https://go.microsoft.com/fwlink/?linkid=2008654)
  
[<span data-ttu-id="deab3-119">เรียนรู้เพิ่มเติมเกี่ยวกับการทํางานกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="deab3-119">Learn more about working with SharePoint groups</span></span>](https://go.microsoft.com/fwlink/?linkid=874658)
  

