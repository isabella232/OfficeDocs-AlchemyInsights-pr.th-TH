---
title: สิทธิ์ของผู้ใช้
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 67aaea23-025c-4af6-a826-bf97cec216ef
ms.openlocfilehash: 779db68e3018476f64da78678766b81cc0656cad
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796739"
---
# <a name="user-permissions-in-sharepoint-and-onedrive"></a><span data-ttu-id="0ecf0-102">สิทธิ์ของผู้ใช้ใน SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="0ecf0-102">User permissions in SharePoint and OneDrive</span></span>

<span data-ttu-id="0ecf0-103">ถ้าผู้ใช้ในองค์กรของคุณไม่สามารถเข้าถึง SharePoint หรือ OneDrive ตรวจสอบให้แน่ใจว่าพวกเขามีสิทธิ์การใช้งานที่มี SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="0ecf0-103">If a user in your organization isn't able to access SharePoint or OneDrive, make sure they have a license that includes SharePoint and OneDrive.</span></span> 
  
1. <span data-ttu-id="0ecf0-104">ไปที่ [หน้าผู้ใช้ที่ใช้งานอยู่ในศูนย์การจัดการ Microsoft ๓๖๕](https://portal.office.com/adminportal/home#/users) แล้วเลือกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="0ecf0-104">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users) and select the user.</span></span> 
    
2. <span data-ttu-id="0ecf0-105">ตรวจสอบให้แน่ใจว่าภายใต้สิทธิ์การใช้งาน **ผลิตภัณฑ์**สิทธิ์การใช้งานจะถูกกำหนดและ **SharePoint Online** ถูกเลือกไว้</span><span class="sxs-lookup"><span data-stu-id="0ecf0-105">Make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
 <span data-ttu-id="0ecf0-106">เมื่อต้องการให้สิทธิ์แก่ผู้ใช้ในการเข้าถึงไซต์ SharePoint ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="0ecf0-106">To give a user permission to access a SharePoint site:</span></span> 
  
1. <span data-ttu-id="0ecf0-107">เปิดไซต์ในเว็บเบราว์เซอร์</span><span class="sxs-lookup"><span data-stu-id="0ecf0-107">Open the site in a web browser.</span></span>
    
2. <span data-ttu-id="0ecf0-108">ถ้าไซต์เป็นสมาชิกของกลุ่ม Microsoft ๓๖๕ให้คลิกไอคอนการตั้งค่าที่มุมขวาบนแล้วคลิก**สิทธิ์สำหรับไซต์**</span><span class="sxs-lookup"><span data-stu-id="0ecf0-108">If the site belongs to a Microsoft 365 group, click the Settings icon in the upper right, and then click **Site permissions**.</span></span> <span data-ttu-id="0ecf0-109">คลิก **เชิญบุคคล**แล้วเลือกเพื่อเพิ่มสมาชิกลงในกลุ่ม Microsoft ๓๖๕หรือแชร์เฉพาะไซต์</span><span class="sxs-lookup"><span data-stu-id="0ecf0-109">Click **Invite people**, and then choose to add members to the Microsoft 365 group or share only the site.</span></span> 
    
    <span data-ttu-id="0ecf0-110">สำหรับไซต์การติดต่อสื่อสารให้คลิก **แชร์ไซต์** ที่มุมขวาบนแล้วใส่ชื่อของบุคคลนั้นแล้วเลือกระดับสิทธิ์ (อ่านแก้ไขหรือควบคุมทั้งหมด)</span><span class="sxs-lookup"><span data-stu-id="0ecf0-110">For a communication site, click **Share site** in the upper-right, enter the person's name, and then select the permission level (Read, Edit, or Full Control).</span></span> 
    
    <span data-ttu-id="0ecf0-111">สำหรับไซต์ทีมคลาสสิกให้คลิก **แชร์** ที่มุมขวาบน</span><span class="sxs-lookup"><span data-stu-id="0ecf0-111">For a classic team site, click **Share** in the upper-right.</span></span> <span data-ttu-id="0ecf0-112">ใส่ชื่อของบุคคลที่คุณต้องการเชิญหรือพิมพ์ทุกคนเพื่อแชร์กับทุกคนในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="0ecf0-112">Enter the name of the person you want to invite or type Everyone to share with everyone in your organization.</span></span> <span data-ttu-id="0ecf0-113">คลิก**แชร์**</span><span class="sxs-lookup"><span data-stu-id="0ecf0-113">Click **Share**.</span></span>
    
> [!NOTE]
> <span data-ttu-id="0ecf0-114">ถ้าคุณเป็นสมาชิกของไซต์แต่ไม่ใช่เจ้าของคุณสามารถเชิญบุคคลอื่นมายังไซต์แต่การเชิญของคุณจะสร้างการร้องขอการเข้าถึงที่สามารถอนุมัติหรือปฏิเสธโดยเจ้าของไซต์ได้</span><span class="sxs-lookup"><span data-stu-id="0ecf0-114">If you're a member of a site but not an owner, you can invite people to the site, but your invitation will generate an access request that can be either approved or declined by a site owner.</span></span> 
  
[<span data-ttu-id="0ecf0-115">เรียนรู้วิธีการแชร์ไฟล์หรือโฟลเดอร์กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="0ecf0-115">Learn how to share a file or folder with a user</span></span>](https://go.microsoft.com/fwlink/?linkid=533408)
  

