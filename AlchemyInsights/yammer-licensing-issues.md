---
title: ปัญหาสิทธิ์การใช้งาน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657295"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="4d6dc-102">ปัญหาสิทธิ์การใช้งาน Yammer</span><span class="sxs-lookup"><span data-stu-id="4d6dc-102">Yammer licensing issues</span></span>

<span data-ttu-id="4d6dc-103">ผู้ใช้ทุกคนต้องมีสิทธิ์การใช้งานในการใช้บริการ Yammer Enterprise แต่ตามค่าเริ่มต้น Yammer ไม่จำเป็นต้องมีสิทธิ์การใช้งานในการเข้าถึงบริการ</span><span class="sxs-lookup"><span data-stu-id="4d6dc-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="4d6dc-104">เมื่อผู้ดูแลระบบเปลี่ยนการตั้งค่าเพื่อบล็อกผู้ใช้ Microsoft ๓๖๕โดยไม่มีสิทธิ์การใช้งาน Yammer ผู้ใช้ที่ไม่ได้กำหนดสิทธิ์การใช้งาน Yammer Enterprise ไม่สามารถเข้าถึงบริการ Yammer ได้</span><span class="sxs-lookup"><span data-stu-id="4d6dc-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="4d6dc-105">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="4d6dc-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="4d6dc-106">เมื่อสิทธิ์การใช้งานถูกเอาออกจากผู้ใช้ไทล์ Yammer จะไม่แสดงอีกต่อไปและบริการอื่นๆสามารถใช้สิทธิ์การเอาสิทธิ์การใช้งานเพื่อซ่อนฟีเจอร์ได้อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="4d6dc-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="4d6dc-107">ในกรณีอื่นๆฟีเจอร์ยังสามารถปรากฏขึ้นได้แต่จำเป็นต้องมีการมอบหมายสิทธิ์การใช้งานเพื่อดำเนินการ</span><span class="sxs-lookup"><span data-stu-id="4d6dc-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="4d6dc-108">**สิทธิ์การใช้งานไม่ได้รับการอัปเดตสำหรับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="4d6dc-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="4d6dc-109">ในบางครั้งผู้ใช้จะได้รับมอบหมายสิทธิ์การใช้งานแต่ยังไม่สามารถเข้าถึง Yammer ได้</span><span class="sxs-lookup"><span data-stu-id="4d6dc-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="4d6dc-110">ความล่าช้ามีแนวโน้มที่จะเกิดขึ้นเมื่อมีการกำหนดสิทธิ์การใช้งานจำนวนมากกำลังดำเนินการอยู่</span><span class="sxs-lookup"><span data-stu-id="4d6dc-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="4d6dc-111">ผู้ใช้ Yammer อาจไม่ได้รับการอัปเดตในลำดับเดียวกันกับสิทธิ์การใช้งานที่มีการเปลี่ยนแปลงใน Azure AD เนื่องจากระบบทำงานแบบอะซิงโครนัส</span><span class="sxs-lookup"><span data-stu-id="4d6dc-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="4d6dc-112">รอจนถึง24ชั่วโมงก่อนที่จะเปิดกรณีสนับสนุนเพื่อรายงานปัญหาการซิงค์สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="4d6dc-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="4d6dc-113">**การมอบหมายสิทธิ์การเป็นกลุ่มจำนวนมาก**</span><span class="sxs-lookup"><span data-stu-id="4d6dc-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="4d6dc-114">สิทธิ์การใช้งานสามารถกำหนดได้ผ่านทางศูนย์การจัดการหรือการเขียนสคริปต์ PowerShell</span><span class="sxs-lookup"><span data-stu-id="4d6dc-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="4d6dc-115">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่กำหนดสิทธิ์การใช้งานให้กับผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)และ[กำหนดสิทธิ์การใช้งานให้กับบัญชีผู้ใช้ด้วย Office ๓๖๕ PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="4d6dc-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="4d6dc-116">ฝ่ายสนับสนุนของไมโครซอฟท์ไม่มีความช่วยเหลือเกี่ยวกับการสร้างสคริปต์แต่เอกสารประกอบบนการกำหนดสิทธิ์การใช้งาน Yammer จะพร้อมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="4d6dc-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="4d6dc-117">สำหรับข้อมูลเพิ่มเติมให้ดูที่[จัดการสิทธิ์การใช้งาน Yammer โดยใช้ Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)</span><span class="sxs-lookup"><span data-stu-id="4d6dc-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>