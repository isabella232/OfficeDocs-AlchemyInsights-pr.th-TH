---
title: ปัญหาการอนุญาตให้ใช้สิทธิ์ Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148426"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="920dc-102">ปัญหาการอนุญาตให้ใช้สิทธิ์ Yammer</span><span class="sxs-lookup"><span data-stu-id="920dc-102">Yammer licensing issues</span></span>

<span data-ttu-id="920dc-103">ผู้ใช้ทั้งหมดต้องมีสิทธิ์การใช้งานเพื่อใช้บริการ Yammer องค์กร แต่โดยค่าเริ่มต้น Yammer ไม่จําเป็นต้องให้ผู้ใช้มีสิทธิ์การใช้งานในการเข้าถึงบริการ</span><span class="sxs-lookup"><span data-stu-id="920dc-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="920dc-104">เมื่อผู้ดูแลระบบเปลี่ยนแปลงการตั้งค่าเพื่อบล็อกผู้ใช้ Microsoft 365 โดยไม่มีสิทธิ์การใช้งาน Yammer ผู้ใช้ไม่ได้กําหนดสิทธิ์การใช้งาน Yammer องค์กรไม่สามารถเข้าถึงบริการ Yammer</span><span class="sxs-lookup"><span data-stu-id="920dc-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="920dc-105">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="920dc-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="920dc-106">เมื่อสิทธิ์การใช้งานจะถูกเอาออกจากผู้ใช้ จะไม่มีแสดงไทล์ Yammer อีกต่อไป และบริการอื่น ๆ สามารถใช้การเอาออกสิทธิ์การใช้งานเพื่อซ่อนลักษณะการทํางาน</span><span class="sxs-lookup"><span data-stu-id="920dc-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="920dc-107">ในกรณีอื่นๆ ฟีเจอร์ยังคงปรากฏอยู่ แต่จําเป็นต้องมีการกําหนดสิทธิ์การใช้งานเพื่อใช้งาน</span><span class="sxs-lookup"><span data-stu-id="920dc-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="920dc-108">**สิทธิ์การใช้งานไม่ได้รับการปรับปรุงสําหรับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="920dc-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="920dc-109">ในบางครั้ง ผู้ใช้จะได้รับมอบหมายสิทธิ์การใช้งาน แต่ยังคงไม่สามารถเข้าถึง Yammer ได้</span><span class="sxs-lookup"><span data-stu-id="920dc-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="920dc-110">ความล่าช้ามีแนวโน้มที่จะเกิดขึ้นเมื่อการมอบหมายใบอนุญาตจํานวนมากกําลังดําเนินการ</span><span class="sxs-lookup"><span data-stu-id="920dc-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="920dc-111">ผู้ใช้ Yammer อาจไม่ได้รับการปรับปรุงในลําดับเดียวกันเป็นสิทธิ์การใช้งานมีการเปลี่ยนแปลงในโฆษณา Azure เนื่องจากระบบทํางานแบบอะซิงโครนัส</span><span class="sxs-lookup"><span data-stu-id="920dc-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="920dc-112">รอถึง 24 ชั่วโมงก่อนที่จะเปิดกรณีการสนับสนุนเพื่อรายงานปัญหาการซิงค์ใบอนุญาต</span><span class="sxs-lookup"><span data-stu-id="920dc-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="920dc-113">**การมอบหมายสิทธิ์การใช้งานจํานวนมาก**</span><span class="sxs-lookup"><span data-stu-id="920dc-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="920dc-114">สิทธิ์การใช้งานสามารถถูกกําหนดผ่านศูนย์การจัดการหรือการเขียนสคริปต์ PowerShell</span><span class="sxs-lookup"><span data-stu-id="920dc-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="920dc-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การกําหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)และ[มอบหมายสิทธิ์การใช้งานให้กับบัญชีผู้ใช้ด้วย Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="920dc-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="920dc-116">ฝ่ายสนับสนุนของ Microsoft ไม่ได้ให้ความช่วยเหลือในการสร้างสคริปต์ แต่เอกสารเกี่ยวกับการกําหนดสิทธิ์การใช้งาน Yammer จะพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="920dc-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="920dc-117">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งาน Yammer โดยใช้ Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)</span><span class="sxs-lookup"><span data-stu-id="920dc-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>