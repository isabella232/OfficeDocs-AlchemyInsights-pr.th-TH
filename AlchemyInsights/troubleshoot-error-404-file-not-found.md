---
title: การแก้ไขปัญหาข้อผิดพลาด๔๐๔ไม่พบไฟล์
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750110"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="1360f-102">การแก้ไขปัญหาข้อผิดพลาด๔๐๔ไม่พบไฟล์</span><span class="sxs-lookup"><span data-stu-id="1360f-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="1360f-103">ข้อผิดพลาด๔๐๔ได้รับเมื่อผู้ใช้พยายามเข้าถึงไซต์หรือไฟล์ใน SharePoint หรือ OneDrive</span><span class="sxs-lookup"><span data-stu-id="1360f-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="1360f-104">ซึ่งมักจะเกิดจากไซต์หรือไฟล์หรือกลุ่มที่ได้รับการเปลี่ยนชื่อย้ายหรือลบออก</span><span class="sxs-lookup"><span data-stu-id="1360f-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="1360f-105">ตัวอย่างเช่น: ผู้ใช้จะพบข้อผิดพลาด๔๐๔ในการพยายามเข้าถึงไซต์คอลเลกชันรากและถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="1360f-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="1360f-106">เมื่อต้องการแก้ไขข้อผิดพลาด๔๐๔สำหรับไซต์ที่ถูกเปลี่ยนชื่อย้ายหรือลบออกให้ดำเนินการดังนี้</span><span class="sxs-lookup"><span data-stu-id="1360f-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="1360f-107">สำหรับไซต์แบบคลาสสิกที่มีอยู่ในศูนย์การจัดการแบบคลาสสิกให้ดูที่[คืนค่าไซต์คอลเลกชันที่ถูกลบ](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="1360f-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="1360f-108">สำหรับไซต์ที่ทันสมัย (การติดต่อสื่อสารกลุ่มที่เชื่อมต่อหรือไซต์อื่นๆ) ที่มีอยู่ในศูนย์การจัดการ SharePoint ใหม่ให้ดูที่[ดูและคืนค่าไซต์ที่ถูกลบในศูนย์การจัดการ sharepoint ใหม่](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)</span><span class="sxs-lookup"><span data-stu-id="1360f-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="1360f-109">เมื่อต้องการแก้ไขข้อผิดพลาด๔๐๔สำหรับไฟล์ (หรือรายการอื่น) ที่ถูกเปลี่ยนชื่อย้ายหรือลบออกให้ดำเนินการดังนี้</span><span class="sxs-lookup"><span data-stu-id="1360f-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="1360f-110">ไปที่ไซต์ SharePoint หรือ OneDrive และดูถังรีไซเคิลจากเนื้อหาของไซต์</span><span class="sxs-lookup"><span data-stu-id="1360f-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="1360f-111">ให้ดู[ที่คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)</span><span class="sxs-lookup"><span data-stu-id="1360f-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="1360f-112">ถ้าคุณยังไม่สามารถค้นหารายการที่คุณสามารถค้นหาบันทึกการตรวจสอบได้ถ้าเปิดใช้งานการบันทึกให้[ค้นหาบันทึกการตรวจสอบในศูนย์การรักษาความปลอดภัย & ของ Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="1360f-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
