---
title: "\"การแก้ไขปัญหาไฟล์หรือโฟลเดอร์ที่หายไป"
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
ms.assetid: 1fab9c5d-f6ca-461c-94f0-76e7cfb8a26d
ms.openlocfilehash: 3b344e7a4a5f663b15a9f3820d1ff7b28ad61b4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670671"
---
# <a name="troubleshooting-missing-files-or-folders-in-onedrive-or-sharepoint"></a><span data-ttu-id="9eb66-102">การแก้ไขปัญหาไฟล์หรือโฟลเดอร์ที่หายไปใน OneDrive หรือ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9eb66-102">Troubleshooting missing Files or Folders in OneDrive or SharePoint</span></span>

- [<span data-ttu-id="9eb66-103">ตรวจสอบถังรีไซเคิลของไซต์</span><span class="sxs-lookup"><span data-stu-id="9eb66-103">Check the recycle bin of the site</span></span>](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)

- [<span data-ttu-id="9eb66-104">การคืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="9eb66-104">Restore items in the Recycle Bin of a SharePoint site</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)



<span data-ttu-id="9eb66-105">**ฟีเจอร์การคืนค่าไฟล์**</span><span class="sxs-lookup"><span data-stu-id="9eb66-105">**Files Restore feature**</span></span>

<span data-ttu-id="9eb66-106">ถ้าไฟล์ OneDrive หรือไฟล์ SharePoint จำนวนมากของคุณได้รับการลบเขียนทับเสียหายหรือติดมัลแวร์คุณสามารถคืนค่าไลบรารี OneDrive หรือ Sharepoint ทั้งหมดของคุณเป็นเวลาก่อนหน้าได้โดยใช้ฟีเจอร์การคืนค่าไฟล์</span><span class="sxs-lookup"><span data-stu-id="9eb66-106">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="9eb66-107">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="9eb66-107">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

- [<span data-ttu-id="9eb66-108">การคืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="9eb66-108">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

<span data-ttu-id="9eb66-109">**ใช้การบันทึกการตรวจสอบหรือบานหน้าต่างกิจกรรมของไฟล์เพื่อตรวจสอบประวัติการทำงานของไฟล์**</span><span class="sxs-lookup"><span data-stu-id="9eb66-109">**Use audit logging or the file activity pane to check history of the file**</span></span>

<span data-ttu-id="9eb66-110">[ตรวจสอบรายงาน](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) </a> การตรวจสอบ โดยการนำทาง[ที่นี่](https://protection.office.com/#/unifiedauditlog)</span><span class="sxs-lookup"><span data-stu-id="9eb66-110">[Check the audit reports](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</a> by navigating [here](https://protection.office.com/#/unifiedauditlog)</span></span>

<span data-ttu-id="9eb66-111">ใช้บานหน้าต่าง [กิจกรรมของไฟล์](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0) เพื่อตรวจสอบประวัติไฟล์</span><span class="sxs-lookup"><span data-stu-id="9eb66-111">Use the [file activity](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0) pane to check the history of the file.</span></span>

<span data-ttu-id="9eb66-112">ตรวจสอบไคลเอ็นต์การซิงค์ OneDrive บนเครื่องภายในเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="9eb66-112">Check the OneDrive Sync Client on your local machine.</span></span>  <span data-ttu-id="9eb66-113">ถ้าคุณกำลังซิงค์ไฟล์บนคอมพิวเตอร์ของคุณผ่านทางไคลเอ็นต์การซิงค์ OneDrive ให้ตรวจสอบโฟลเดอร์การซิงค์ภายในเครื่องเพื่อให้แน่ใจว่าได้อัปโหลดอย่างถูกต้องแล้ว</span><span class="sxs-lookup"><span data-stu-id="9eb66-113">If you're syncing the files on your computer via OneDrive Sync client, check the local sync folder to ensure that it has been properly uploaded.</span></span> <span data-ttu-id="9eb66-114">ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบถังรีไซเคิลบนเครื่องภายในเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="9eb66-114">Ensure you also check the recycle bin on your local machine.</span></span>



