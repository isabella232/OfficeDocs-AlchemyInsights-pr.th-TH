---
title: การแก้ไขปัญหาข้อผิดพลาด 404 ไม่พบไฟล์
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 467feb3cb436a2e0135162657876e5c45d8d56bd
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243764"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="6c62d-102">การแก้ไขปัญหาข้อผิดพลาด 404 ไม่พบไฟล์</span><span class="sxs-lookup"><span data-stu-id="6c62d-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="6c62d-103">404 เพราะข้อผิดพลาดได้รับเมื่อผู้ใช้พยายามเข้าถึงไซต์หรือแฟ้มใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="6c62d-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="6c62d-104">ซึ่งมักมีสาเหตุมาจากไซต์ หรือแฟ้ม หรือกลุ่มการเปลี่ยนชื่อ ย้าย หรือลบ</span><span class="sxs-lookup"><span data-stu-id="6c62d-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="6c62d-105">ตัวอย่าง: ผู้ใช้จะพบข้อผิดพลาด 404 พยายามเข้าถึงไซต์คอลเลกชันราก และได้ถูกลบไป</span><span class="sxs-lookup"><span data-stu-id="6c62d-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="6c62d-106">เมื่อต้องการแก้ไขข้อผิดพลาด 404 สำหรับไซต์ที่ถูกเปลี่ยนชื่อ ย้าย หรือลบออก:</span><span class="sxs-lookup"><span data-stu-id="6c62d-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="6c62d-107">สำหรับไซต์แบบคลาสสิกที่มีอยู่ในศูนย์กลางการดูแลแบบคลาสสิก ดู[คืนค่าคอลเลกชันของไซต์ที่ถูกลบไปแล้ว](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="6c62d-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="6c62d-108">สำหรับสมัยใหม่ไซต์ (ไซต์อื่น ๆ หรือการสื่อสาร กลุ่มการเชื่อมต่อ ) ที่มีอยู่ในศูนย์กลางการดูแล SharePoint ใหม่ ดู[มุมมองและการคืนค่าลบไซต์ในศูนย์กลางการดูแล SharePoint ใหม่](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="6c62d-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="6c62d-109">เมื่อต้องการแก้ไข 404 เพราะข้อผิดพลาดสำหรับแฟ้ม (หรือรายการอื่น) ที่ถูกเปลี่ยนชื่อ ย้าย หรือลบออก:</span><span class="sxs-lookup"><span data-stu-id="6c62d-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="6c62d-110">ไปยังไซต์ SharePoint หรือ OneDrive และดูถังรีไซเคิลจากเนื้อหาของไซต์</span><span class="sxs-lookup"><span data-stu-id="6c62d-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="6c62d-111">ดู[เรียกคืนรายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)</span><span class="sxs-lookup"><span data-stu-id="6c62d-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="6c62d-112">ถ้าคุณยังคงไม่สามารถค้นหารายการคุณสามารถค้นหาบันทึกการตรวจสอบถ้าการเข้าสู่ระบบถูกเปิดใช้งาน เท่านั้น[ค้นหาตรวจสอบล็อกใน & Office 365 Security Center การปฏิบัติตามกฎระเบียบ](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)</span><span class="sxs-lookup"><span data-stu-id="6c62d-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
