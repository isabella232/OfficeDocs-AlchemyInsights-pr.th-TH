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
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797567"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="09ea1-102">คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="09ea1-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="09ea1-103">SharePoint Online จะเก็บข้อมูลสำรองของเนื้อหาทั้งหมดสำหรับ14วันเพิ่มเติมเกินกว่าการลบที่แท้จริง</span><span class="sxs-lookup"><span data-stu-id="09ea1-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="09ea1-104">ถ้าไม่สามารถคืนค่าเนื้อหาผ่านถังรีไซเคิลหรือคืนค่าไฟล์ผู้ดูแลระบบสามารถติดต่อฝ่ายสนับสนุนของ Microsoft เพื่อขอคืนค่าได้ตลอดเวลาภายในหน้าต่าง14วัน</span><span class="sxs-lookup"><span data-stu-id="09ea1-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="09ea1-105">บูรณะจากการสำรองข้อมูลสามารถทำให้เสร็จสมบูรณ์สำหรับไซต์คอลเลกชันหรือไซต์ย่อยเท่านั้นไม่ใช่สำหรับไฟล์รายการหรือไลบรารีที่เฉพาะเจาะจงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="09ea1-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="09ea1-106">เมื่อคุณลบรายการหรือไซต์ออกจาก Sharepoint ไฟล์นั้นจะไม่ถูกเอาออกทันที</span><span class="sxs-lookup"><span data-stu-id="09ea1-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="09ea1-107">รายการที่ถูกลบไปยังถังรีไซเคิลเป็นระยะเวลาหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="09ea1-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="09ea1-108">ในระหว่างช่วงเวลานั้นคุณสามารถคืนค่ารายการที่คุณลบไปยังตำแหน่งที่ตั้งเดิมได้</span><span class="sxs-lookup"><span data-stu-id="09ea1-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="09ea1-109">สำหรับข้อมูลเพิ่มเติมโปรดไปที่ลิงก์ด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="09ea1-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="09ea1-110">[คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)</span><span class="sxs-lookup"><span data-stu-id="09ea1-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="09ea1-111">คืนค่าไฟล์หรือโฟลเดอร์ที่ถูกลบใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="09ea1-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="09ea1-112">คืนค่าไซต์คอลเลกชันที่ถูกลบ (รวมถึงกลุ่มการสื่อสารและไซต์อื่นๆ)</span><span class="sxs-lookup"><span data-stu-id="09ea1-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="09ea1-113">การคืนค่าไซต์ OneDrive ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="09ea1-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="09ea1-114">สำหรับการดำเนินการถังรีไซเคิลเป็นกลุ่มผู้ดูแลระบบอาจพิจารณาใช้[Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="09ea1-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="09ea1-115">**ฟีเจอร์การคืนค่าไฟล์**</span><span class="sxs-lookup"><span data-stu-id="09ea1-115">**Files Restore feature**</span></span>

<span data-ttu-id="09ea1-116">ถ้าไฟล์ OneDrive หรือไฟล์ SharePoint จำนวนมากของคุณได้รับการลบเขียนทับเสียหายหรือติดมัลแวร์คุณสามารถคืนค่าไลบรารี OneDrive หรือ SharePoint ทั้งหมดของคุณเป็นเวลาก่อนหน้าได้โดยใช้ฟีเจอร์การคืนค่าไฟล์</span><span class="sxs-lookup"><span data-stu-id="09ea1-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="09ea1-117">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="09ea1-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="09ea1-118">การคืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="09ea1-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

