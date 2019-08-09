---
title: คืนค่าโฟลเดอร์หรือแฟ้มที่ถูกลบไปแล้ว
ms.author: efrene
author: efrene
ms.date: 8/6/2019
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.custom:
- "9000210"
- "1782"
ms.openlocfilehash: e6c16b7bf94ded492ef54c00b4967f78ee4bcf1c
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270655"
---
# <a name="restore-deleted-items-from-sharepoint"></a><span data-ttu-id="6cb68-102">คืนค่าลบรายการจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="6cb68-102">Restore deleted items from SharePoint</span></span>

<span data-ttu-id="6cb68-103">เมื่อคุณลบสินค้าหรือไซต์จาก Sharepoint จึงไม่ได้ทันทีเอาออก</span><span class="sxs-lookup"><span data-stu-id="6cb68-103">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="6cb68-104">รายการที่ถูกลบไปไว้ในถังรีไซเคิลสำหรับรอบระยะเวลา</span><span class="sxs-lookup"><span data-stu-id="6cb68-104">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="6cb68-105">ในช่วงเวลานั้น คุณสามารถคืนค่ารายการคุณลบไปตำแหน่งที่ตั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="6cb68-105">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="6cb68-106">สำหรับข้อมูลเพิ่มเติมโปรดเยี่ยมชมลิงค์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="6cb68-106">For more information please visit the links below.</span></span>

- <span data-ttu-id="6cb68-107">[คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US)</span><span class="sxs-lookup"><span data-stu-id="6cb68-107">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

- [<span data-ttu-id="6cb68-108">ลบการคืนค่าแฟ้มหรือโฟลเดอร์ใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="6cb68-108">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

- [<span data-ttu-id="6cb68-109">ลบรายการ หรือลบข้อมูลใน'ถังรีไซเคิล'</span><span class="sxs-lookup"><span data-stu-id="6cb68-109">Delete items or empty the Recycle Bin</span></span>](https://support.office.com/article/delete-items-or-empty-the-recycle-bin-of-a-sharepoint-site-2e713599-d13e-40d6-96dc-66f0a366f74e#ID0EAADAAA=Online)

- <span data-ttu-id="6cb68-110">[คืนค่าลบไซต์คอลเลกชัน (รวมทั้งกลุ่ม การสื่อสาร และไซต์อื่น ๆ)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection )</span><span class="sxs-lookup"><span data-stu-id="6cb68-110">[Restore a deleted site collection (Including group, communication and other sites)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection ).</span></span>

- [<span data-ttu-id="6cb68-111">คืนค่า OneDrive ถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="6cb68-111">Restore a deleted OneDrive</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

- [<span data-ttu-id="6cb68-112">PNP ออนไลน์ของ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6cb68-112">SharePoint Online PNP</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)

<span data-ttu-id="6cb68-113">**คุณลักษณะการคืนค่าแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="6cb68-113">**Files Restore feature**</span></span>

<span data-ttu-id="6cb68-114">ถ้าล็อตของแฟ้ม OneDrive หรือ Sharepoint ของคุณได้รับลบ เขียนทับ เสียหาย หรือการติดไวรัส โดยมัลแวร์ คุณสามารถคืนค่ารี OneDrive หรือ Sharepoint ของคุณทั้งหมดไปยังเวลาก่อนหน้าโดยใช้คุณลักษณะการคืนค่าแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="6cb68-114">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="6cb68-115">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="6cb68-115">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a150)

- [<span data-ttu-id="6cb68-116">คืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="6cb68-116">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US)
