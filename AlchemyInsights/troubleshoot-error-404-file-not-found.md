---
title: แก้ไขปัญหาข้อผิดพลาด 404 ไม่พบแฟ้ม
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: ed35c790dfb048aa6f33fa439b7636864a6e6e6c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759783"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="1845b-102">แก้ไขปัญหาข้อผิดพลาด 404 ไม่พบแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="1845b-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="1845b-103">ข้อผิดพลาด 404 ได้รับเมื่อผู้ใช้พยายามเข้าถึงไซต์หรือแฟ้มใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="1845b-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="1845b-104">ซึ่งมักเกิดจากไซต์หรือแฟ้มหรือกลุ่มการเปลี่ยนชื่อ ย้าย หรือลบ</span><span class="sxs-lookup"><span data-stu-id="1845b-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="1845b-105">ตัวอย่างเช่น: ผู้ใช้จะพบข้อผิดพลาด 404 พยายามเข้าถึงคอลเลกชันไซต์ราก และถูกลบ</span><span class="sxs-lookup"><span data-stu-id="1845b-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="1845b-106">เมื่อต้องการแก้ไขข้อผิดพลาด 404 สําหรับไซต์ที่ถูกเปลี่ยนชื่อ ย้าย หรือถูกลบ:</span><span class="sxs-lookup"><span data-stu-id="1845b-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="1845b-107">สําหรับไซต์คลาสสิกที่มีอยู่ในศูนย์การจัดการแบบคลาสสิก ให้ดูที่[การคืนค่าไซต์คอลเลกชันที่ถูกลบ](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="1845b-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="1845b-108">สําหรับไซต์สมัยใหม่ (การติดต่อสื่อสาร ที่เชื่อมต่อกลุ่ม หรือไซต์อื่นๆ) ที่มีอยู่ในศูนย์การจัดการ SharePoint ใหม่ ให้ดูที่[การดูและคืนค่าไซต์ที่ถูกลบในศูนย์การจัดการ SharePoint ใหม่](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="1845b-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="1845b-109">เมื่อต้องการแก้ไขข้อผิดพลาด 404 สําหรับแฟ้ม (หรือรายการอื่น ๆ) ที่ถูกเปลี่ยนชื่อ ย้าย หรือถูกลบ:</span><span class="sxs-lookup"><span data-stu-id="1845b-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="1845b-110">ไปที่ไซต์ SharePoint หรือ OneDrive และดูถังรีไซเคิลจากเนื้อหาของไซต์</span><span class="sxs-lookup"><span data-stu-id="1845b-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="1845b-111">ดู[คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)</span><span class="sxs-lookup"><span data-stu-id="1845b-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="1845b-112">ถ้าคุณยังคงไม่สามารถค้นหารายการคุณสามารถค้นหาบันทึกการตรวจสอบถ้าเปิดใช้งานการบันทึกดู[ค้นหาบันทึกการตรวจสอบใน Microsoft 365 Security &ศูนย์ปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)</span><span class="sxs-lookup"><span data-stu-id="1845b-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
