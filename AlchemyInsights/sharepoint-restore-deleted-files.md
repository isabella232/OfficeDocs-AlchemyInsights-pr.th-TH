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
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707541"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="223ba-102">คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="223ba-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="223ba-103">SharePoint Online เก็บรักษาการสํารองข้อมูลเนื้อหาทั้งหมดไว้เป็นเวลา 14 วันนอกเหนือจากการลบจริง</span><span class="sxs-lookup"><span data-stu-id="223ba-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="223ba-104">ถ้าไม่สามารถคืนค่าเนื้อหาผ่านทางถังรีไซเคิลหรือการคืนค่าไฟล์ ได้ ผู้ดูแลระบบสามารถติดต่อฝ่ายสนับสนุนของไมโครซอฟท์เพื่อขอคืนค่าได้ตลอดเวลาภายในหน้าต่าง 14 วัน</span><span class="sxs-lookup"><span data-stu-id="223ba-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="223ba-105">การคืนค่าจากการสํารองข้อมูลสามารถเสร็จสมบูรณ์ได้เฉพาะกับไซต์คอลเลกชันหรือไซต์ย่อยเท่านั้น ไม่ใช่ไฟล์ รายการ หรือไลบรารีที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="223ba-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="223ba-106">เมื่อคุณลบรายการหรือไซต์ออกจาก SharePoint รายการนั้นจะไม่ถูกเอาออกทันที</span><span class="sxs-lookup"><span data-stu-id="223ba-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="223ba-107">Deleted items go into the recycle bin for a period of time.</span><span class="sxs-lookup"><span data-stu-id="223ba-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="223ba-108">ในระหว่างช่วงเวลาดังกล่าว คุณสามารถคืนค่ารายการที่คุณลบไปยังสถานที่เดิมได้</span><span class="sxs-lookup"><span data-stu-id="223ba-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="223ba-109">หากต้องการข้อมูลเพิ่มเติม โปรดไปที่ลิงก์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="223ba-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="223ba-110">[คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="223ba-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="223ba-111">คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="223ba-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="223ba-112">คืนค่าไซต์คอลเลกชันที่ถูกลบ (รวมถึงกลุ่ม การติดต่อสื่อสารและไซต์อื่นๆ)</span><span class="sxs-lookup"><span data-stu-id="223ba-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="223ba-113">คืนค่าไซต์ OneDrive ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="223ba-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="223ba-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="223ba-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="223ba-115">**ฟีเจอร์การคืนค่าไฟล์**</span><span class="sxs-lookup"><span data-stu-id="223ba-115">**Files Restore feature**</span></span>

<span data-ttu-id="223ba-116">ถ้าไฟล์ OneDrive หรือ SharePoint ของคุณถูกลบ ถูกเขียนทับ เสียหาย หรือติดมัลแวร์ คุณสามารถคืนค่าไลบรารี OneDrive หรือ SharePoint ทั้งหมดของคุณในครั้งก่อนหน้าได้โดยใช้ฟีเจอร์คืนค่าไฟล์</span><span class="sxs-lookup"><span data-stu-id="223ba-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="223ba-117">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="223ba-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="223ba-118">คืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="223ba-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

