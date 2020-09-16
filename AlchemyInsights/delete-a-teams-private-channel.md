---
title: การลบแชนเนลส่วนตัวของทีม
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730934"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="a7f75-102">การลบแชนเนลส่วนตัวของทีม</span><span class="sxs-lookup"><span data-stu-id="a7f75-102">Delete a Teams private channel</span></span>

<span data-ttu-id="a7f75-103">Microsoft ทราบถึงปัญหาในการลบทีมส่วนตัวถ้าคุณมีนโยบายการเก็บข้อมูล SharePoint ที่เปิดใช้งานสำหรับไซต์ SharePoint ต้นแบบ</span><span class="sxs-lookup"><span data-stu-id="a7f75-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="a7f75-104">Microsoft กำลังทำงานกับการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="a7f75-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="a7f75-105">ในระหว่างนี้คุณสามารถใช้วิธีการแก้ไขปัญหาต่อไปนี้เพื่อลบช่องทางส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="a7f75-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="a7f75-106">**ยกเว้นไซต์คอลเลกชันของทีม/ไซต์คอลเลกชันจากนโยบายการเก็บข้อมูลของ Sharepoint**</span><span class="sxs-lookup"><span data-stu-id="a7f75-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="a7f75-107">ไปที่พอร์ทัลผู้ดูแลระบบ Office ๓๖๕แล้วเลือก **แสดงทั้งหมด** ในบานหน้าต่างนำทางด้านซ้าย</span><span class="sxs-lookup"><span data-stu-id="a7f75-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="a7f75-108">ภายใต้**ศูนย์การจัดการ**ให้ไปที่นโยบายการป้องกันการสูญหายของข้อมูลการ**รักษาความปลอดภัย & การปฏิบัติ**ตามนโยบาย  >  **Data Loss Prevention**  >  **Policy**</span><span class="sxs-lookup"><span data-stu-id="a7f75-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="a7f75-109">ระบุนโยบายใดๆที่นำไปใช้กับไซต์ Sharepoint และปรับเปลี่ยนนโยบายดังนั้นไซต์ Sharepoint สำหรับทีมที่มีแชนเนลส่วนตัวจะไม่รวมอยู่ภายใต้นโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="a7f75-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="a7f75-110">บันทึกนโยบาย</span><span class="sxs-lookup"><span data-stu-id="a7f75-110">Save the policy.</span></span>
    <span data-ttu-id="a7f75-111">อาจใช้เวลาถึง24ชั่วโมงสำหรับการตั้งค่านโยบายจะมีผล</span><span class="sxs-lookup"><span data-stu-id="a7f75-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="a7f75-112">หลังจากที่ไซต์ถูกแยกออกแล้วคุณสามารถลบแชนเนลส่วนตัวได้</span><span class="sxs-lookup"><span data-stu-id="a7f75-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="a7f75-113">คุณ  ***อาจ*** สามารถลบช่องทางส่วนตัวโดยใช้ทีม Microsoft บนอุปกรณ์ Android ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a7f75-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="a7f75-114">สำหรับข้อมูล SharePoint ที่เกี่ยวข้องให้ดูที่ [ไม่สามารถลบรายการใน SharePoint Online หรือ OneDrive For Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)ได้</span><span class="sxs-lookup"><span data-stu-id="a7f75-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>