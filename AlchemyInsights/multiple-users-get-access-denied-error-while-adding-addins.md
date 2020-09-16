---
title: ผู้ใช้หลายคนได้รับข้อผิดพลาดในการปฏิเสธการเข้าถึงในขณะที่เพิ่ม add-in ใน Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724382"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="9b417-102">ผู้ใช้หลายคนได้รับข้อผิดพลาดในการปฏิเสธการเข้าถึงในขณะที่เพิ่ม add-in ใน Outlook</span><span class="sxs-lookup"><span data-stu-id="9b417-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="9b417-103">คุณสามารถระบุว่าผู้ดูแลระบบใดในองค์กรของคุณมีสิทธิ์ในการติดตั้งและจัดการ add-in สำหรับ Outlook</span><span class="sxs-lookup"><span data-stu-id="9b417-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="9b417-104">นอกจากนี้คุณยังสามารถระบุผู้ใช้ที่อยู่ในองค์กรของคุณได้รับสิทธิ์ในการติดตั้งและจัดการ add-in สำหรับการใช้งานของตนเอง</span><span class="sxs-lookup"><span data-stu-id="9b417-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="9b417-105">สำหรับรายละเอียดให้ดู [ที่ระบุผู้ดูแลระบบและผู้ใช้ที่สามารถติดตั้งและจัดการ add-in สำหรับ Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)ได้</span><span class="sxs-lookup"><span data-stu-id="9b417-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="9b417-106">เมื่อต้องการตรวจสอบว่าคุณได้กำหนดสิทธิ์สำหรับผู้ใช้ให้แทนที่ <Role Name> ด้วยชื่อของบทบาทเพื่อตรวจสอบและเรียกใช้คำสั่งต่อไปนี้ใน Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9b417-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="9b417-107">รับ-ManagementRoleAssignment-บทบาท " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="9b417-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="9b417-108">ตัวอย่างนี้จะแสดงให้คุณเห็นวิธีการตรวจสอบว่าคุณได้กำหนดสิทธิ์ในการติดตั้ง add-in จาก Office Store สำหรับองค์กรหรือไม่</span><span class="sxs-lookup"><span data-stu-id="9b417-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="9b417-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="9b417-109">PowerShell</span></span>

<span data-ttu-id="9b417-110">-บทบาท "แอป Org Marketplace"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="9b417-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="9b417-111">ในผลลัพธ์ที่ได้รับ ManagementRoleAssignment ให้ตรวจทานรายการในคอลัมน์ผู้ใช้ที่มีประสิทธิภาพ</span><span class="sxs-lookup"><span data-stu-id="9b417-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="9b417-112">สำหรับรายละเอียดเกี่ยวกับไวยากรณ์และพารามิเตอร์ข้อมูลให้ดูที่[รับ ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)</span><span class="sxs-lookup"><span data-stu-id="9b417-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 