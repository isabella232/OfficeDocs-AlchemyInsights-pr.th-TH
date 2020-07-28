---
title: ลบแชนเนลส่วนตัวของทีม
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439912"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="e4e2d-102">ลบแชนเนลส่วนตัวของทีม</span><span class="sxs-lookup"><span data-stu-id="e4e2d-102">Delete a Teams private channel</span></span>

<span data-ttu-id="e4e2d-103">Microsoft ตระหนักถึงปัญหาในการลบแชนเนลส่วนตัวของ Teams ถ้าคุณมีนโยบายการเก็บข้อมูล SharePoint ที่เปิดใช้งานสําหรับไซต์ SharePoint ต้นแบบ</span><span class="sxs-lookup"><span data-stu-id="e4e2d-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="e4e2d-104">ไมโครซอฟท์กําลังทํางานเกี่ยวกับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="e4e2d-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="e4e2d-105">ในระหว่างนี้ คุณสามารถใช้วิธีแก้ปัญหาต่อไปนี้เพื่อลบสถานีส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="e4e2d-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="e4e2d-106">**แยกชุดทีม/ไซต์ออกจากนโยบายการเก็บข้อมูลของ Sharepoint**</span><span class="sxs-lookup"><span data-stu-id="e4e2d-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="e4e2d-107">ไปที่พอร์ทัลผู้ดูแลระบบ Office 365 แล้วเลือก**แสดงทั้งหมด**ในบานหน้าต่างนําทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="e4e2d-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="e4e2d-108">ภายใต้**ศูนย์การจัดการ**ให้ไปที่**นโยบายการป้องกัน**  >  **การสูญหายของข้อมูล**  >  **Policy**&การปฏิบัติตามกฎระเบียบ</span><span class="sxs-lookup"><span data-stu-id="e4e2d-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="e4e2d-109">ระบุนโยบายใด ๆ ที่ใช้กับไซต์ Sharepoint และปรับเปลี่ยนนโยบายเพื่อให้ไซต์ Sharepoint สําหรับทีมที่มีแชนเนลส่วนตัวไม่ได้รวมอยู่ในนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="e4e2d-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="e4e2d-110">บันทึกนโยบาย</span><span class="sxs-lookup"><span data-stu-id="e4e2d-110">Save the policy.</span></span>
    <span data-ttu-id="e4e2d-111">การตั้งค่านโยบายอาจใช้เวลาถึง 24 ชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="e4e2d-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="e4e2d-112">หลังจากที่เว็บไซต์ได้รับการยกเว้นคุณสามารถลบช่องส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="e4e2d-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="e4e2d-113">***คุณอาจ***ลบช่องส่วนตัวได้โดยใช้ Microsoft Teams บนอุปกรณ์ Android ของคุณ</span><span class="sxs-lookup"><span data-stu-id="e4e2d-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="e4e2d-114">สําหรับข้อมูล SharePoint ที่เกี่ยวข้อง ให้ดูที่[ไม่สามารถลบรายการใน SharePoint แบบออนไลน์ หรือ OneDrive สําหรับธุรกิจ](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)</span><span class="sxs-lookup"><span data-stu-id="e4e2d-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>