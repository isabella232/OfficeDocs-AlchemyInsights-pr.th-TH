---
title: "\"การแก้ไขปัญหาแฟ้มหรือโฟลเดอร์ที่หายไป"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1fab9c5d-f6ca-461c-94f0-76e7cfb8a26d
ms.openlocfilehash: a3e3fa3cbaf3ab3c1fcf42e8a564d2b7cd8428eb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511239"
---
# <a name="troubleshooting-missing-files-or-folders-in-onedrive-or-sharepoint"></a><span data-ttu-id="6b689-102">การแก้ไขปัญหาแฟ้มหรือโฟลเดอร์ที่หายไปใน OneDrive หรือ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b689-102">Troubleshooting missing Files or Folders in OneDrive or SharePoint</span></span>

- [<span data-ttu-id="6b689-103">ตรวจสอบถังรีไซเคิลของไซต์</span><span class="sxs-lookup"><span data-stu-id="6b689-103">Check the recycle bin of the site</span></span>](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)

- [<span data-ttu-id="6b689-104">การคืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="6b689-104">Restore items in the Recycle Bin of a SharePoint site</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)



<span data-ttu-id="6b689-105">**คุณลักษณะการคืนค่าแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="6b689-105">**Files Restore feature**</span></span>

<span data-ttu-id="6b689-106">ถ้าไฟล์ OneDrive หรือ SharePoint ของคุณจํานวนมากถูกลบ เขียนทับ เสียหาย หรือติดไวรัสโดยมัลแวร์ คุณสามารถกู้คืนไลบรารี OneDrive หรือ Sharepoint ทั้งหมดของคุณกลับไปเป็นครั้งก่อนหน้าโดยใช้คุณลักษณะการกู้คืนไฟล์</span><span class="sxs-lookup"><span data-stu-id="6b689-106">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="6b689-107">คืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="6b689-107">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

- [<span data-ttu-id="6b689-108">การคืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="6b689-108">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

<span data-ttu-id="6b689-109">**ใช้การบันทึกการตรวจสอบหรือบานหน้าต่างกิจกรรมไฟล์เพื่อตรวจสอบประวัติของไฟล์**</span><span class="sxs-lookup"><span data-stu-id="6b689-109">**Use audit logging or the file activity pane to check history of the file**</span></span>

<span data-ttu-id="6b689-110">[ตรวจสอบรายงานการตรวจสอบ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) </a> โดยการนําทาง[ที่นี่](https://protection.office.com/#/unifiedauditlog)</span><span class="sxs-lookup"><span data-stu-id="6b689-110">[Check the audit reports](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</a> by navigating [here](https://protection.office.com/#/unifiedauditlog)</span></span>

<span data-ttu-id="6b689-111">ใช้บานหน้าต่าง[กิจกรรมไฟล์](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0)เพื่อตรวจสอบประวัติของแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="6b689-111">Use the [file activity](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0) pane to check the history of the file.</span></span>

<span data-ttu-id="6b689-112">ตรวจสอบไคลเอ็นต์การซิงค์ OneDrive บนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="6b689-112">Check the OneDrive Sync Client on your local machine.</span></span>  <span data-ttu-id="6b689-113">ถ้าคุณกําลังซิงค์ไฟล์ในคอมพิวเตอร์ของคุณผ่านทางไคลเอ็นต์ OneDrive Sync ให้ตรวจสอบโฟลเดอร์การซิงค์ภายในเครื่องเพื่อให้แน่ใจว่าไฟล์นั้นได้รับการอัปโหลดอย่างถูกต้องแล้ว</span><span class="sxs-lookup"><span data-stu-id="6b689-113">If you're syncing the files on your computer via OneDrive Sync client, check the local sync folder to ensure that it has been properly uploaded.</span></span> <span data-ttu-id="6b689-114">ตรวจสอบให้แน่ใจว่าคุณตรวจสอบถังรีไซเคิลบนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="6b689-114">Ensure you also check the recycle bin on your local machine.</span></span>



