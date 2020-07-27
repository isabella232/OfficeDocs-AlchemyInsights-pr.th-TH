---
title: ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424177"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="66593-102">ผู้ใช้หลายคนได้รับข้อผิดพลาดการเข้าถึงถูกปฏิเสธในขณะที่เพิ่ม Add-in ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="66593-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="66593-103">คุณสามารถระบุผู้ดูแลระบบในองค์กรของคุณมีสิทธิ์ในการติดตั้งและจัดการ Add-in สําหรับ Outlook</span><span class="sxs-lookup"><span data-stu-id="66593-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="66593-104">คุณยังสามารถระบุผู้ใช้ในองค์กรของคุณที่มีสิทธิ์ในการติดตั้งและจัดการ Add-in สําหรับการใช้ของตนเอง</span><span class="sxs-lookup"><span data-stu-id="66593-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="66593-105">สําหรับรายละเอียด ให้ดูที่[ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ Add-in สําหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="66593-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="66593-106">เมื่อต้องการตรวจสอบว่า คุณได้กําหนดสิทธิ์สําหรับผู้ใช้เสร็จเรียบร้อยแล้ว ให้แทนที่ <Role Name> ด้วยชื่อของบทบาทเพื่อตรวจสอบ และเรียกใช้คําสั่งต่อไปนี้ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน:</span><span class="sxs-lookup"><span data-stu-id="66593-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="66593-107">รับการจัดการการจัดระเบียบ -บทบาท <Role Name> "" -GetประสิทธิภาพUsers</span><span class="sxs-lookup"><span data-stu-id="66593-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="66593-108">ตัวอย่างนี้แสดงวิธีการตรวจสอบว่าคุณได้กําหนดสิทธิ์ให้ใครติดตั้ง Add-in จาก Office Store สําหรับองค์กร</span><span class="sxs-lookup"><span data-stu-id="66593-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="66593-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="66593-109">PowerShell</span></span>

<span data-ttu-id="66593-110">บทบาท "Org Marketplace Apps" - Getประสิทธิภาพการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="66593-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="66593-111">ในผลลัพธ์ที่ได้รับการจัดการรายงานการตรวจสอบรายการในคอลัมน์ผู้ใช้ที่มีประสิทธิภาพ</span><span class="sxs-lookup"><span data-stu-id="66593-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="66593-112">สําหรับข้อมูลไวยากรณ์และพารามิเตอร์โดยละเอียด ให้ดูที่[รับการจัดการการมอบหมาย](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)</span><span class="sxs-lookup"><span data-stu-id="66593-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 