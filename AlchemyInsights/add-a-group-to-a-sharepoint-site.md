---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 07850bc8c496df180d2e3c85dfbfc999231f6a54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697360"
---
# <a name="add-a-group-to-a-sharepoint-site"></a><span data-ttu-id="82b5f-102">เพิ่มกลุ่มลงในไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="82b5f-102">Add a group to a SharePoint site</span></span>

<span data-ttu-id="82b5f-103">ไซต์ทีม SharePoint บางไซต์ (รวมถึงที่สร้างขึ้นในทีม Microsoft) จะได้รับการจัดการโดยเจ้าของกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="82b5f-103">Some SharePoint team sites (including those created in Microsoft Teams) are managed by Microsoft 365 group owners.</span></span> <span data-ttu-id="82b5f-104">ไซต์ SharePoint และเนื้อหายังสามารถแชร์กับกลุ่ม Microsoft ๓๖๕และกับกลุ่ม SharePoint ได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="82b5f-104">SharePoint sites and content can also be shared with Microsoft 365 groups, and with SharePoint groups.</span></span> <span data-ttu-id="82b5f-105">กลุ่ม SharePoint คือคอลเลกชันของผู้ใช้ที่มีสิทธิ์การใช้งานไซต์และเนื้อหาเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="82b5f-105">A SharePoint group is a collection of users who all have the same set of permissions to sites and content.</span></span> <span data-ttu-id="82b5f-106">สำหรับไซต์คลาสสิกเราขอแนะนำให้คุณใช้กลุ่มเพื่อกำหนดระดับสิทธิ์เดียวกันให้กับผู้ใช้หลายคนในครั้งเดียวแทนที่จะกำหนดสิทธิ์ให้กับผู้ใช้หนึ่งคนในแต่ละครั้ง</span><span class="sxs-lookup"><span data-stu-id="82b5f-106">For classic sites, we recommend that you use groups to conveniently assign the same permission level to many people at once rather than assigning permissions one person at a time.</span></span>
  
<span data-ttu-id="82b5f-107">จัดการสมาชิกของกลุ่ม Microsoft ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="82b5f-107">Manage Microsoft 365 group members:</span></span>
  
1. <span data-ttu-id="82b5f-108">ไปที่[หน้ากลุ่มในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="82b5f-108">Go to the [Groups page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="82b5f-109">เลือกกลุ่มเพื่อดูเจ้าของและสมาชิก</span><span class="sxs-lookup"><span data-stu-id="82b5f-109">Select a group to see its owners and members.</span></span> <span data-ttu-id="82b5f-110">เมื่อต้องการเพิ่มหรือเอาบุคคลออกให้คลิกลิงก์**แก้ไข**ในแถว**เจ้าของ**หรือ**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="82b5f-110">To add or remove people, click the **Edit** link in the **Owners** or **Members** row.</span></span> 
    
<span data-ttu-id="82b5f-111">แชร์ไซต์การติดต่อสื่อสารกับกลุ่ม Microsoft ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="82b5f-111">Share a communication site with a Microsoft 365 group:</span></span>
  
1. <span data-ttu-id="82b5f-112">ไปที่ไซต์ในเบราว์เซอร์แล้วคลิก **แชร์ไซต์** ที่มุมขวาบน</span><span class="sxs-lookup"><span data-stu-id="82b5f-112">Go to the site in a browser and click **Share site** in the upper right.</span></span> 
    
2. <span data-ttu-id="82b5f-113">ใส่ชื่อกลุ่มแล้วเลือกระดับสิทธิ์ (อ่านแก้ไขหรือควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="82b5f-113">Enter the group name, and then select the permission level (Read, Edit, or Full Control).</span></span>
    
<span data-ttu-id="82b5f-114">สร้างกลุ่ม SharePoint เพื่อใช้กับไซต์แบบคลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="82b5f-114">Create a SharePoint group to use with a classic site:</span></span>
  
1. <span data-ttu-id="82b5f-115">ไปที่ไซต์ในเบราว์เซอร์แล้วคลิกไอคอนการตั้งค่าที่มุมขวาบน</span><span class="sxs-lookup"><span data-stu-id="82b5f-115">Go to the site in a browser and click the Settings icon in the upper right.</span></span>
    
2. <span data-ttu-id="82b5f-116">คลิก**การตั้งค่าไซต์**จากนั้นภายใต้**ผู้ใช้และสิทธิ์**ให้คลิก**สิทธิ์สำหรับไซต์**</span><span class="sxs-lookup"><span data-stu-id="82b5f-116">Click **Site settings**, and then under **Users and Permissions**, click **Site permissions**.</span></span>
    
3. <span data-ttu-id="82b5f-117">บนแท็บสิทธิ์ให้คลิก**สร้างกลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="82b5f-117">On the Permissions tab, click **Create Group**.</span></span>
    
[<span data-ttu-id="82b5f-118">เชื่อมต่อไซต์ทีมคลาสสิกกับกลุ่ม Microsoft ๓๖๕ใหม่</span><span class="sxs-lookup"><span data-stu-id="82b5f-118">Connect a classic team site to a new Microsoft 365 group</span></span>](https://go.microsoft.com/fwlink/?linkid=2008654)
  
[<span data-ttu-id="82b5f-119">เรียนรู้เพิ่มเติมเกี่ยวกับการทำงานกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="82b5f-119">Learn more about working with SharePoint groups</span></span>](https://go.microsoft.com/fwlink/?linkid=874658)
  

