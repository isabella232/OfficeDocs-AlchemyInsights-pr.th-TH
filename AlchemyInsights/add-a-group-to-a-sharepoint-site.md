---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495230"
---
# <a name="add-a-group-to-a-sharepoint-site"></a><span data-ttu-id="16d26-102">เพิ่มกลุ่มลงในไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="16d26-102">Add a group to a SharePoint site</span></span>

<span data-ttu-id="16d26-103">บางไซต์ทีม SharePoint (รวมทั้งที่สร้างขึ้นใน Microsoft ทีม) จะถูกจัดการ โดยเจ้าของกลุ่ม Office 365</span><span class="sxs-lookup"><span data-stu-id="16d26-103">Some SharePoint team sites (including those created in Microsoft Teams) are managed by Office 365 group owners.</span></span> <span data-ttu-id="16d26-104">ไซต์ SharePoint และเนื้อหาสามารถนอกจากนี้ยังสามารถใช้ร่วม กับกลุ่ม Office 365 และกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="16d26-104">SharePoint sites and content can also be shared with Office 365 groups, and with SharePoint groups.</span></span> <span data-ttu-id="16d26-105">กลุ่ม SharePoint คือ คอลเลกชันของผู้ใช้ทั้งหมดได้รับการสิทธิ์ไปยังไซต์และเนื้อหาชุดเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="16d26-105">A SharePoint group is a collection of users who all have the same set of permissions to sites and content.</span></span> <span data-ttu-id="16d26-106">สำหรับไซต์คลาสสิค เราขอแนะนำให้ คุณใช้กลุ่มเพื่อกำหนดระดับสิทธิ์เดียวกันในแต่ละครั้งให้ผู้รับหลายคนพร้อมกันแทนที่จะกำหนดสิทธิ์หนึ่งคนได้อย่างสะดวก</span><span class="sxs-lookup"><span data-stu-id="16d26-106">For classic sites, we recommend that you use groups to conveniently assign the same permission level to many people at once rather than assigning permissions one person at a time.</span></span>
  
<span data-ttu-id="16d26-107">จัดการสมาชิกกลุ่ม Office 365:</span><span class="sxs-lookup"><span data-stu-id="16d26-107">Manage Office 365 group members:</span></span>
  
1. <span data-ttu-id="16d26-108">ไป[หน้ากลุ่มใน Microsoft 365 admin ศูนย์](https://portal.office.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="16d26-108">Go to the [Groups page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/groups).</span></span>
    
2. <span data-ttu-id="16d26-109">เลือกเพื่อดูเจ้าของและสมาชิกของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="16d26-109">Select a group to see its owners and members.</span></span> <span data-ttu-id="16d26-110">การเพิ่ม หรือเอาบุคคล คลิก**แก้ไข**การเชื่อมโยงในแถว**เจ้าของ**หรือ**สมาชิก**</span><span class="sxs-lookup"><span data-stu-id="16d26-110">To add or remove people, click the **Edit** link in the **Owners** or **Members** row.</span></span> 
    
<span data-ttu-id="16d26-111">ไซต์การสื่อสารที่ใช้ร่วมกันกับกลุ่มที่มี Office 365:</span><span class="sxs-lookup"><span data-stu-id="16d26-111">Share a communication site with an Office 365 group:</span></span>
  
1. <span data-ttu-id="16d26-112">ไปไซต์ในเบราว์เซอร์ และคลิก**ไซต์ที่ใช้ร่วมกัน**ในมุมขวาด้านบน</span><span class="sxs-lookup"><span data-stu-id="16d26-112">Go to the site in a browser and click **Share site** in the upper right.</span></span> 
    
2. <span data-ttu-id="16d26-113">ป้อนชื่อกลุ่ม และจากนั้น เลือกระดับสิทธิ์ (อ่าน แก้ไข หรือ ควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="16d26-113">Enter the group name, and then select the permission level (Read, Edit, or Full Control).</span></span>
    
<span data-ttu-id="16d26-114">สร้างกลุ่ม SharePoint จะใช้กับไซต์คลาสสิก:</span><span class="sxs-lookup"><span data-stu-id="16d26-114">Create a SharePoint group to use with a classic site:</span></span>
  
1. <span data-ttu-id="16d26-115">ไปไซต์ในเบราว์เซอร์ และคลิกไอคอนการตั้งค่าในมุมขวาด้านบน</span><span class="sxs-lookup"><span data-stu-id="16d26-115">Go to the site in a browser and click the Settings icon in the upper right.</span></span>
    
2. <span data-ttu-id="16d26-116">คลิกการ**ตั้งค่าไซต์**และจากนั้น ภายใต้**ผู้ใช้และสิทธิ์**คลิก**สิทธิ์ของไซต์**</span><span class="sxs-lookup"><span data-stu-id="16d26-116">Click **Site settings**, and then under **Users and Permissions**, click **Site permissions**.</span></span>
    
3. <span data-ttu-id="16d26-117">บนแท็บสิทธิ์ คลิก**สร้าง กลุ่ม**</span><span class="sxs-lookup"><span data-stu-id="16d26-117">On the Permissions tab, click **Create Group**.</span></span>
    
[<span data-ttu-id="16d26-118">ไซต์ทีม classic การเชื่อมต่อไปยังกลุ่มใหม่ของ Office 365</span><span class="sxs-lookup"><span data-stu-id="16d26-118">Connect a classic team site to a new Office 365 group</span></span>](https://go.microsoft.com/fwlink/?linkid=2008654)
  
[<span data-ttu-id="16d26-119">เรียนรู้เพิ่มเติมเกี่ยวกับการทำงานกับกลุ่ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="16d26-119">Learn more about working with SharePoint groups</span></span>](https://go.microsoft.com/fwlink/?linkid=874658)
  

