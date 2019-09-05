---
title: "\"การแก้ไขปัญหาแฟ้มหรือโฟลเดอร์ที่หายไป"
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1fab9c5d-f6ca-461c-94f0-76e7cfb8a26d
ms.openlocfilehash: c5f9d50cc95b1dfeddad1cf6f9d141a7c0d876ad
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750755"
---
# <a name="troubleshooting-missing-files-or-folders-in-onedrive-or-sharepoint"></a><span data-ttu-id="ed634-102">การแก้ไขปัญหาแฟ้มหรือโฟลเดอร์ที่หายไปใน OneDrive หรือ SharePoint</span><span class="sxs-lookup"><span data-stu-id="ed634-102">Troubleshooting missing Files or Folders in OneDrive or SharePoint</span></span>

- [<span data-ttu-id="ed634-103">ตรวจสอบถังรีไซเคิลของไซต์</span><span class="sxs-lookup"><span data-stu-id="ed634-103">Check the recycle bin of the site</span></span>](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)

- [<span data-ttu-id="ed634-104">การคืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="ed634-104">Restore items in the Recycle Bin of a SharePoint site</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)



<span data-ttu-id="ed634-105">**คุณลักษณะการคืนค่าแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="ed634-105">**Files Restore feature**</span></span>

<span data-ttu-id="ed634-106">ถ้าจำนวนมากของ OneDrive หรือแฟ้ม SharePoint ของคุณได้รับการลบการเขียนทับเสียหายหรือติดเชื้อโดยมัลแวร์คุณสามารถคืนค่าทั้ง OneDrive หรือไลบรารี Sharepoint ของคุณไปยังเวลาก่อนหน้านี้โดยใช้คุณลักษณะการคืนค่าแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="ed634-106">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

- [<span data-ttu-id="ed634-107">การคืนค่าไลบรารี OneDrive</span><span class="sxs-lookup"><span data-stu-id="ed634-107">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

- [<span data-ttu-id="ed634-108">การคืนค่าไลบรารีเอกสาร</span><span class="sxs-lookup"><span data-stu-id="ed634-108">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

<span data-ttu-id="ed634-109">**ใช้บันทึกการตรวจสอบหรือบานหน้าต่างกิจกรรมของแฟ้มเพื่อตรวจสอบประวัติของแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="ed634-109">**Use audit logging or the file activity pane to check history of the file**</span></span>

<span data-ttu-id="ed634-110">[ตรวจสอบรายงาน](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fen-us%252farticle%252fsearch-the-audit-log-in-the-office-365-protection-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)</a>การตรวจสอบโดยการนำทางที่[นี่](https://protection.office.com/#/unifiedauditlog)</span><span class="sxs-lookup"><span data-stu-id="ed634-110">[Check the audit reports](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fen-us%252farticle%252fsearch-the-audit-log-in-the-office-365-protection-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)</a> by navigating [here](https://protection.office.com/#/unifiedauditlog)</span></span>

<span data-ttu-id="ed634-111">ใช้บานหน้าต่าง[กิจกรรมแฟ้ม](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0)เพื่อตรวจสอบประวัติของแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="ed634-111">Use the [file activity](https://support.office.com/article/File-activity-in-a-document-library-6105ecda-1dd0-4f6f-9542-102bf5c0ffe0) pane to check the history of the file.</span></span>

<span data-ttu-id="ed634-112">ตรวจสอบไคลเอ็นต์การซิงค์ OneDrive บนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="ed634-112">Check the OneDrive Sync Client on your local machine.</span></span>  <span data-ttu-id="ed634-113">ถ้าคุณกำลังซิงค์แฟ้มบนคอมพิวเตอร์ของคุณผ่านทางไคลเอ็นต์การซิงค์ OneDrive ให้ตรวจสอบโฟลเดอร์ซิงค์ภายในเครื่องเพื่อให้แน่ใจว่าได้อัปโหลดอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="ed634-113">If you're syncing the files on your computer via OneDrive Sync client, check the local sync folder to ensure that it has been properly uploaded.</span></span> <span data-ttu-id="ed634-114">ให้แน่ใจว่าคุณได้ตรวจสอบถังรีไซเคิลบนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="ed634-114">Ensure you also check the recycle bin on your local machine.</span></span>



