---
title: คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.custom:
- "9000210"
- "1782"
ms.openlocfilehash: b7bf64c009235bc1dbd3e922296ff6c4bb239450
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708297"
---
# <a name="restore-deleted-items-from-sharepoint"></a><span data-ttu-id="170c4-102">คืนค่ารายการที่ถูกลบจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="170c4-102">Restore deleted items from SharePoint</span></span>

<span data-ttu-id="170c4-103">เมื่อคุณลบรายการหรือไซต์ออกจาก SharePoint รายการนั้นจะไม่ถูกเอาออกทันที</span><span class="sxs-lookup"><span data-stu-id="170c4-103">When you delete an item or site from SharePoint, it isn't immediately removed.</span></span> <span data-ttu-id="170c4-104">Deleted items go into the recycle bin for a period of time.</span><span class="sxs-lookup"><span data-stu-id="170c4-104">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="170c4-105">ในระหว่างช่วงเวลาดังกล่าว คุณสามารถคืนค่ารายการที่คุณลบไปยังสถานที่เดิมได้</span><span class="sxs-lookup"><span data-stu-id="170c4-105">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="170c4-106">หากต้องการข้อมูลเพิ่มเติม โปรดไปที่ลิงก์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="170c4-106">For more information please visit the links below.</span></span>

- [<span data-ttu-id="170c4-107">คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="170c4-107">Restore items in the Recycle Bin of a SharePoint site</span></span>](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)

- [<span data-ttu-id="170c4-108">คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="170c4-108">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

- [<span data-ttu-id="170c4-109">ลบรายการหรือล้างถังรีไซเคิล</span><span class="sxs-lookup"><span data-stu-id="170c4-109">Delete items or empty the Recycle Bin</span></span>](https://support.office.com/article/delete-items-or-empty-the-recycle-bin-of-a-sharepoint-site-2e713599-d13e-40d6-96dc-66f0a366f74e#ID0EAADAAA=Online)

- <span data-ttu-id="170c4-110">[คืนค่าไซต์คอลเลกชันที่ถูกลบ (รวมถึงกลุ่ม การติดต่อสื่อสารและไซต์อื่นๆ)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection )</span><span class="sxs-lookup"><span data-stu-id="170c4-110">[Restore a deleted site collection (Including group, communication and other sites)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection ).</span></span>

- [<span data-ttu-id="170c4-111">คืนค่า OneDrive ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="170c4-111">Restore a deleted OneDrive</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

- [<span data-ttu-id="170c4-112">SharePoint Online PNP</span><span class="sxs-lookup"><span data-stu-id="170c4-112">SharePoint Online PNP</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)

<span data-ttu-id="170c4-113">**ฟีเจอร์การคืนค่าไฟล์**</span><span class="sxs-lookup"><span data-stu-id="170c4-113">**Files Restore feature**</span></span>

<span data-ttu-id="170c4-114">ถ้าไฟล์ OneDrive หรือ SharePoint ของคุณถูกลบ ถูกเขียนทับ เสียหาย หรือติดมัลแวร์ คุณสามารถคืนค่าไลบรารี OneDrive หรือ SharePoint ทั้งหมดของคุณในครั้งก่อนหน้าได้โดยใช้ฟีเจอร์คืนค่าไฟล์</span><span class="sxs-lookup"><span data-stu-id="170c4-114">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="170c4-115">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="170c4-115">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a150)

- [<span data-ttu-id="170c4-116">คืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="170c4-116">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)
