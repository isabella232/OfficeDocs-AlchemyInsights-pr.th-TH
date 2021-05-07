---
title: การปรับใช้ Add-in Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233553"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="c2f75-102">การปรับใช้ Add-in Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="c2f75-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="c2f75-103">การปรับใช้แบบรวมศูนย์เป็นวิธีที่แนะOffice Add-in กับผู้ใช้และกลุ่มภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="c2f75-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="c2f75-104">เมื่อต้องการปรับใช้ Add-in ให้ปฏิบัติตามขั้นตอนด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="c2f75-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="c2f75-105">**หมายเหตุ:** เมื่อต้องการติดตั้ง Add-in Officeเป็นผู้ใช้แต่ละราย [ให้ดู ดู จัดการ และติดตั้ง Add-in](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)Officeต่างๆ</span><span class="sxs-lookup"><span data-stu-id="c2f75-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="c2f75-106">นอกจากนี้ ตรวจสอบให้แน่ใจว่าได้เปิดใช้งานการรับ add-in Office Store แต่ละรายการแล้ว</span><span class="sxs-lookup"><span data-stu-id="c2f75-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="c2f75-107">For details, see [Prevent add-in downloads by off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span><span class="sxs-lookup"><span data-stu-id="c2f75-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="c2f75-108">ตรวจสอบให้แน่ใจว่าสภาพแวดล้อมของคุณตรงตามความต้องการในการปรับใช้ Add-in โดยใช้การปรับใช้แบบรวมศูนย์</span><span class="sxs-lookup"><span data-stu-id="c2f75-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="c2f75-109">โปรดดูรายละเอียดที่[ข้อกฎหมาย](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="c2f75-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="c2f75-110">ไปที่ **การตั้งค่า**  >  **แอปที่**  >  **รวมรับ** แอปในศูนย์Microsoft 365การจัดการเพื่อปรับใช้ Add-in</span><span class="sxs-lookup"><span data-stu-id="c2f75-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="c2f75-111">หมายเหตุ:</span><span class="sxs-lookup"><span data-stu-id="c2f75-111">Notes:</span></span> 

- <span data-ttu-id="c2f75-112">แอปที่รวมต้องการให้ผู้ดูแลระบบมีสิทธิ์ผู้ดูแลระบบส่วนกลางExchangeสิทธิ์ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="c2f75-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="c2f75-113">เมื่อปรับใช้ Add-in กับผู้ใช้หลายราย เราขอแนะนนะให้มอบหมายโดยใช้กลุ่มแทนผู้ใช้แต่ละราย</span><span class="sxs-lookup"><span data-stu-id="c2f75-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="c2f75-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="c2f75-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="c2f75-115">การปรับใช้แบบรวมศูนย์ไม่สนับสนุนผู้ใช้ในกลุ่มที่ซ้อนกันหรือกลุ่มที่มีกลุ่มหลัก</span><span class="sxs-lookup"><span data-stu-id="c2f75-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="c2f75-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="c2f75-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="c2f75-117">ตรวจสอบให้แน่ใจว่า บริการการจัดการแอป Microsoft 365 (GUID: '0517ffa1-825d-4aff-9991-3f2336b8a20a') เปิดใช้งานอยู่เพื่อให้ผู้ใช้ลงชื่อเข้าใช้ได้</span><span class="sxs-lookup"><span data-stu-id="c2f75-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="c2f75-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="c2f75-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="c2f75-119">ถ้าคุณพบปัญหาในการปรับใช้ Add-in โดยใช้แอปที่รวม ให้ลองปรับใช้[โดยใช้ Add-in](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="c2f75-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="c2f75-120">สำหรับข้อมูลเพิ่มเติม ให้ดู:</span><span class="sxs-lookup"><span data-stu-id="c2f75-120">For more information, see:</span></span>

<span data-ttu-id="c2f75-121">[ปรับใช้ Add-in ในศูนย์การจัดการ](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [จัดการ Add-in ในศูนย์การจัดการ](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [ใช้ cmdlet PowerShell ของการปรับใช้แบบรวมศูนย์เพื่อจัดการ Add-in](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [เผยแพร่Office Add-in โดยใช้การปรับใช้จากส่วนกลางผ่านทางMicrosoft 365การจัดการ](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [การแก้ไขปัญหา: ผู้ใช้ไม่เห็น Add-in](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [การแก้ไขปัญหาข้อผิดพลาดผู้ใช้ที่มีOffice Add-in](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="c2f75-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>