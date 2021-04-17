---
title: Teams อนุญาตหรือปิดใช้งานวิดีโอ IP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826362"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="dd328-102">Teams อนุญาตหรือปิดใช้งานวิดีโอ IP</span><span class="sxs-lookup"><span data-stu-id="dd328-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="dd328-103">**เปลี่ยนหรือสร้างนโยบายการประชุม**</span><span class="sxs-lookup"><span data-stu-id="dd328-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="dd328-104">เมื่อต้องการเปลี่ยนหรือสร้างนโยบายการประชุม ให้ไปที่ ศูนย์การจัดการ **Microsoft Teams >การประชุม>การประชุม**</span><span class="sxs-lookup"><span data-stu-id="dd328-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="dd328-105">เลือกนโยบายจากรายการ หรือ **คลิก** เพิ่ม</span><span class="sxs-lookup"><span data-stu-id="dd328-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="dd328-106">ถ้าคุณสร้างนโยบายใหม่ ให้เพิ่มชื่อและรายละเอียด</span><span class="sxs-lookup"><span data-stu-id="dd328-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="dd328-107">ชื่อต้องไม่มีอักขระพิเศษหรือยาวเกิน 64 อักขระ</span><span class="sxs-lookup"><span data-stu-id="dd328-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="dd328-108">เลือกการตั้งค่าของคุณ **แล้วคลิก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="dd328-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="dd328-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span><span class="sxs-lookup"><span data-stu-id="dd328-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="dd328-110">คุณจะสร้างนโยบายแบบใหม่ที่ชื่อว่า "แบนด์วิดท์ที่จํากัด" และปิดใช้งานการตั้งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="dd328-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="dd328-111">ภายใต้ **วิดีโอ&เสียง**:</span><span class="sxs-lookup"><span data-stu-id="dd328-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="dd328-112">ปิด อนุญาตการบันทึกระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="dd328-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="dd328-113">ปิดอนุญาตวิดีโอ IP</span><span class="sxs-lookup"><span data-stu-id="dd328-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="dd328-114">จากนั้นกําหนดนโยบายให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="dd328-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="dd328-115">**กําหนดนโยบายการประชุมให้กับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="dd328-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="dd328-116">ในการนําทางด้านซ้ายของศูนย์การจัดการ Microsoft Teams **ให้ไปที่** ผู้ใช้ แล้วคลิกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="dd328-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="dd328-117">เลือกผู้ใช้โดยการคลิกที่ด้านซ้ายของชื่อผู้ใช้ จากนั้นคลิก **แก้ไข** การตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="dd328-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="dd328-118">**ภายใต้ นโยบาย** การประชุม ให้เลือกนโยบายที่คุณต้องการกําหนด แล้วคลิก **ปรับใช้**</span><span class="sxs-lookup"><span data-stu-id="dd328-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="dd328-119">ดูข้อมูลเพิ่มเติมที่[จัดการนโยบายการประชุมใน Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="dd328-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
