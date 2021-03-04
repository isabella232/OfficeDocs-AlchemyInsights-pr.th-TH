---
title: ส่งออก eDiscovery/ผลลัพธ์การค้นหาเนื้อหา
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429975"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="e588c-102">ส่งออก eDiscovery/ผลลัพธ์การค้นหาเนื้อหา</span><span class="sxs-lookup"><span data-stu-id="e588c-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="e588c-103">คุณอาจต้องส่งออกผลลัพธ์การค้นหาของคุณเป็นไฟล์ PST (จากอีเมล) หรือไปยังเอกสาร Office ดั้งเดิม (จากไซต์ SharePoint และ OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="e588c-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="e588c-104">ถ้าเป็นดังนั้น ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e588c-104">If so, do the following:</span></span>

- <span data-ttu-id="e588c-105">ตรวจสอบให้แน่ใจว่าบัญชีของคุณได้รับมอบหมายสิทธิ์ที่เหมาะสมในการส่งออก</span><span class="sxs-lookup"><span data-stu-id="e588c-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="e588c-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span><span class="sxs-lookup"><span data-stu-id="e588c-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="e588c-107">ตรวจสอบให้แน่ใจว่าคอมพิวเตอร์ของคุณตรงตามเงื่อนไข [เบื้องต้น](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="e588c-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="e588c-108">เบราว์เซอร์บางรายการไม่ได้รับการสนับสนุน เช่น Chrome</span><span class="sxs-lookup"><span data-stu-id="e588c-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="e588c-109">เมื่อต้องการส่งออกจากการค้นหาเนื้อหา: a.</span><span class="sxs-lookup"><span data-stu-id="e588c-109">To export from a Content Search: a.</span></span> <span data-ttu-id="e588c-110">ไปที่ศูนย์ [&การปฏิบัติตาม](https://protection.office.com/contentsearch) นโยบาย **แล้วคลิก** ค้นหา **แล้วเลือกการค้นหา** เนื้อหา</span><span class="sxs-lookup"><span data-stu-id="e588c-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="e588c-111">บนหน้า **การค้นหา** เนื้อหา ให้เลือกการค้นหาที่บันทึกไว้</span><span class="sxs-lookup"><span data-stu-id="e588c-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="e588c-112">b.</span><span class="sxs-lookup"><span data-stu-id="e588c-112">b.</span></span> <span data-ttu-id="e588c-113">บนบานหน้าต่างรายละเอียด ภายใต้ **ส่งออกผลลัพธ์ไปยังคอมพิวเตอร์** เลือก **เริ่ม** ส่งออก</span><span class="sxs-lookup"><span data-stu-id="e588c-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="e588c-114">ถ้าคุณส่งออกกล่องจดหมายมากกว่า 100K คุณจะต้องใช้ PowerShell เพื่อดาวน์โหลดผลลัพธ์การส่งออก</span><span class="sxs-lookup"><span data-stu-id="e588c-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="e588c-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span><span class="sxs-lookup"><span data-stu-id="e588c-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="e588c-116">เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู ส่งออกผลลัพธ์การค้นหา](https://go.microsoft.com/fwlink/?linkid=2102118)เนื้อหา</span><span class="sxs-lookup"><span data-stu-id="e588c-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>