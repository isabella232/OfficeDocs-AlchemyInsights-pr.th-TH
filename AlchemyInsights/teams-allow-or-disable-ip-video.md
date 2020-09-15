---
title: ทีมอนุญาตหรือปิดใช้งานวิดีโอ IP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670203"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="a810e-102">ทีมอนุญาตหรือปิดใช้งานวิดีโอ IP</span><span class="sxs-lookup"><span data-stu-id="a810e-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="a810e-103">**เปลี่ยนหรือสร้างนโยบายการประชุม**</span><span class="sxs-lookup"><span data-stu-id="a810e-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="a810e-104">เมื่อต้องการเปลี่ยนแปลงหรือสร้างนโยบายการประชุมให้ไปที่**ศูนย์การจัดการทีม Microsoft > การประชุม > นโยบายการประชุม**</span><span class="sxs-lookup"><span data-stu-id="a810e-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="a810e-105">เลือกนโยบายจากรายการหรือคลิก**เพิ่ม**</span><span class="sxs-lookup"><span data-stu-id="a810e-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="a810e-106">ถ้าคุณกำลังสร้างนโยบายใหม่ให้เพิ่มชื่อและคำอธิบาย</span><span class="sxs-lookup"><span data-stu-id="a810e-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="a810e-107">ชื่อไม่สามารถมีอักขระพิเศษหรือมีความยาวเกินกว่าอักขระ๖๔ได้</span><span class="sxs-lookup"><span data-stu-id="a810e-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="a810e-108">เลือกการตั้งค่าของคุณแล้วคลิก**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="a810e-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="a810e-109">ตัวอย่างเช่นสมมติว่าคุณมีผู้ใช้หลายคนและคุณต้องการจำกัดจำนวนแบนด์วิดธ์ที่การประชุมของพวกเขาจำเป็นต้องใช้</span><span class="sxs-lookup"><span data-stu-id="a810e-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="a810e-110">คุณจะสร้างนโยบายแบบกำหนดเองใหม่ที่ชื่อว่า "แบนด์วิดธ์ที่จำกัด" และปิดใช้งานการตั้งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a810e-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="a810e-111">ภายใต้ **วิดีโอ & เสียง**:</span><span class="sxs-lookup"><span data-stu-id="a810e-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="a810e-112">ปิดใช้งานการบันทึกบนคลาวด์</span><span class="sxs-lookup"><span data-stu-id="a810e-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="a810e-113">ปิดใช้งานการอนุญาตให้ใช้งานวิดีโอ IP</span><span class="sxs-lookup"><span data-stu-id="a810e-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="a810e-114">จากนั้นกำหนดนโยบายให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a810e-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="a810e-115">**กำหนดนโยบายการประชุมให้กับผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="a810e-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="a810e-116">ในการนำทางด้านซ้ายของศูนย์การจัดการทีมของ Microsoft ให้ไปที่ **ผู้ใช้**แล้วคลิกผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a810e-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="a810e-117">เลือกผู้ใช้ด้วยการคลิกที่ด้านซ้ายของชื่อผู้ใช้แล้วคลิก**แก้ไขการตั้งค่า**</span><span class="sxs-lookup"><span data-stu-id="a810e-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="a810e-118">ภายใต้**นโยบายการประชุม**ให้เลือกนโยบายที่คุณต้องการกำหนดแล้วคลิก**นำไปใช้**</span><span class="sxs-lookup"><span data-stu-id="a810e-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="a810e-119">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการนโยบายการประชุมในทีม](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="a810e-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
