---
title: กู้คืนไฟล์หรือโฟลเดอร์ที่ถูกลบ
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 544e65430cce72329933933927883521b2d79e7c
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666139"
---
# <a name="restore-deleted-items-from-sharepoint"></a><span data-ttu-id="59a9c-102">คืนค่ารายการที่ถูกลบจาก SharePoint</span><span class="sxs-lookup"><span data-stu-id="59a9c-102">Restore deleted items from SharePoint</span></span>

<span data-ttu-id="59a9c-103">เมื่อคุณลบรายการหรือไซต์ออกจาก Sharepoint จะไม่มีการเอาออกทันที</span><span class="sxs-lookup"><span data-stu-id="59a9c-103">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="59a9c-104">รายการที่ถูกลบจะเข้าไปในถังรีไซเคิลสำหรับรอบระยะเวลาหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="59a9c-104">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="59a9c-105">ในระหว่างนั้นคุณสามารถคืนค่ารายการที่คุณลบไปยังตำแหน่งที่ตั้งเดิมได้</span><span class="sxs-lookup"><span data-stu-id="59a9c-105">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="59a9c-106">สำหรับข้อมูลเพิ่มเติมโปรดไปที่ลิงก์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="59a9c-106">For more information please visit the links below.</span></span>

- [<span data-ttu-id="59a9c-107">การคืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="59a9c-107">Restore items in the Recycle Bin of a SharePoint site</span></span>](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="59a9c-108">กู้คืนไฟล์หรือโฟลเดอร์ที่ถูกลบใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="59a9c-108">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

- [<span data-ttu-id="59a9c-109">ลบรายการหรือล้างข้อมูลในถังรีไซเคิล</span><span class="sxs-lookup"><span data-stu-id="59a9c-109">Delete items or empty the Recycle Bin</span></span>](https://support.office.com/article/delete-items-or-empty-the-recycle-bin-of-a-sharepoint-site-2e713599-d13e-40d6-96dc-66f0a366f74e#ID0EAADAAA=Online)

- <span data-ttu-id="59a9c-110">[กู้คืนชุดเก็บรวบรวมไซต์ที่ถูกลบ (รวมถึงกลุ่มการสื่อสารและไซต์อื่นๆ)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection )</span><span class="sxs-lookup"><span data-stu-id="59a9c-110">[Restore a deleted site collection (Including group, communication and other sites)](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection ).</span></span>

- [<span data-ttu-id="59a9c-111">กู้คืน OneDrive ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="59a9c-111">Restore a deleted OneDrive</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

- [<span data-ttu-id="59a9c-112">SharePoint แบบออนไลน์ PNP</span><span class="sxs-lookup"><span data-stu-id="59a9c-112">SharePoint Online PNP</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)

<span data-ttu-id="59a9c-113">**คุณลักษณะการคืนค่าแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="59a9c-113">**Files Restore feature**</span></span>

<span data-ttu-id="59a9c-114">ถ้ามีการลบแฟ้ม OneDrive หรือไฟล์ Sharepoint จำนวนมากของคุณจะถูกเอาออกถูกเขียนทับเสียหายหรือติดเชื้อโดยมัลแวร์คุณสามารถคืนค่าทั้ง OneDrive หรือไลบรารี Sharepoint ของคุณไปเป็นครั้งก่อนหน้าโดยใช้คุณลักษณะการคืนค่าแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="59a9c-114">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="59a9c-115">การคืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="59a9c-115">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a150)

- [<span data-ttu-id="59a9c-116">การคืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="59a9c-116">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US)
