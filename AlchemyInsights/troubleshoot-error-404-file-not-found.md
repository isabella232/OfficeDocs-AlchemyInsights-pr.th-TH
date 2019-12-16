---
title: แก้ปัญหาข้อผิดพลาด๔๐๔, ไม่พบแฟ้ม
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 6c23d7c482e3beb900d6e0e2ba596c1ab1db8d7e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050688"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="791fb-102">แก้ปัญหาข้อผิดพลาด๔๐๔, ไม่พบแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="791fb-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="791fb-103">มีข้อผิดพลาด๔๐๔จะได้รับเมื่อผู้ใช้กำลังพยายามเข้าถึงไซต์หรือแฟ้มใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="791fb-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="791fb-104">ซึ่งมักเกิดจากไซต์หรือแฟ้มหรือกลุ่มได้รับการเปลี่ยนชื่อย้ายหรือลบ</span><span class="sxs-lookup"><span data-stu-id="791fb-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="791fb-105">ตัวอย่างเช่นผู้ใช้จะพบข้อผิดพลาด๔๐๔ที่พยายามเข้าถึงไซต์คอลเลกชันรากและถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="791fb-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="791fb-106">การแก้ไขข้อผิดพลาด๔๐๔สำหรับไซต์ที่ถูกเปลี่ยนชื่อย้ายหรือลบ:</span><span class="sxs-lookup"><span data-stu-id="791fb-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="791fb-107">สำหรับเว็บไซต์คลาสสิกที่มีอยู่ในศูนย์ดูแล Classic โปรดดูที่[คืนค่าไซต์คอลเลกชันที่ถูกลบ](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="791fb-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="791fb-108">สำหรับไซต์ที่ทันสมัย (การสื่อสารการเชื่อมต่อกลุ่มหรือไซต์อื่นๆ) ที่มีอยู่ในศูนย์ดูแล SharePoint ใหม่โปรดดูที่[ดูและเรียกคืนไซต์ที่ถูกลบในศูนย์ดูแล sharepoint ใหม่](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="791fb-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="791fb-109">การแก้ไขข้อผิดพลาด๔๐๔สำหรับแฟ้ม (หรือรายการอื่น) ที่ถูกเปลี่ยนชื่อย้ายหรือลบ:</span><span class="sxs-lookup"><span data-stu-id="791fb-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="791fb-110">ไปยังไซต์ SharePoint หรือ OneDrive และดูถังรีไซเคิลจากเนื้อหาของไซต์</span><span class="sxs-lookup"><span data-stu-id="791fb-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="791fb-111">ดู[คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)</span><span class="sxs-lookup"><span data-stu-id="791fb-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="791fb-112">ถ้าคุณยังไม่สามารถค้นหารายการที่คุณสามารถค้นหาแฟ้มบันทึกการตรวจสอบถ้าเปิดใช้งานการเข้าสู่ระบบให้[ค้นหาบันทึกการตรวจสอบใน Office ๓๖๕ความปลอดภัยศูนย์ปฏิบัติตามกฎระเบียบ &](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)</span><span class="sxs-lookup"><span data-stu-id="791fb-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
