---
title: ปัญหาทั่วไปของ SharePoint แบบออนไลน์และวิธีแก้ปัญหา
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: e6b21d4d457cacf1666a74751d285cf09a8833ea
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508406"
---
# <a name="sharepoint-online-common-issues-and-resolutions"></a><span data-ttu-id="eca08-102">ปัญหาทั่วไปของ SharePoint แบบออนไลน์และวิธีแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="eca08-102">SharePoint Online common issues and resolutions</span></span>

<span data-ttu-id="eca08-103">ดูเหมือนว่าคุณถูกถามเกี่ยวกับ SharePoint</span><span class="sxs-lookup"><span data-stu-id="eca08-103">It looks like you are asking about SharePoint.</span></span> <span data-ttu-id="eca08-104">เราสามารถช่วยให้ มีคำตอบที่ชัดเจนยิ่งขึ้นถ้าคุณสั้น ๆ เรียบเรียงคำถามของคุณ ด้วยหนึ่ง หรือสองประโยคที่อธิบายถึงปัญหาของคุณ - รวมทั้งข้อผิดพลาด คุณลักษณะที่คุณกำลังใช้ เป็นต้น ...</span><span class="sxs-lookup"><span data-stu-id="eca08-104">We can help with a more precise answer if you briefly rephrase your question with one or two sentences that describe your issue - including errors, features you're using, etc..</span></span> 

<span data-ttu-id="eca08-105">ในขณะ คือหัวข้อที่ร้องขอบ่อยที่นี่:</span><span class="sxs-lookup"><span data-stu-id="eca08-105">In the meantime here are some frequently requested topics:</span></span>





- <span data-ttu-id="eca08-106">**สิทธิ์**:[สิทธิ์กลยุทธ์การสร้าง](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)และการ[ทำความเข้าใจเกี่ยวกับระดับสิทธิ์](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="eca08-106">**Permissions**: [Build a Permissions strategy](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) and [Understand Permission Levels](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

- <span data-ttu-id="eca08-107">**ใช้ร่วมกัน**:[การใช้งานร่วมกันกับผู้อื่น](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)ภายในองค์กรหรือของคุณ[กับผู้อื่นภายนอกองค์กรของคุณ](https://docs.microsoft.com/sharepoint/external-sharing-overview)</span><span class="sxs-lookup"><span data-stu-id="eca08-107">**Sharing**: [Sharing with others](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) inside your organization or [with others outside your organization](https://docs.microsoft.com/sharepoint/external-sharing-overview).</span></span>

- <span data-ttu-id="eca08-108">**ทำงานกับแฟ้มเอกสาร**: การเรียนรู้เพิ่มเติมเกี่ยวกับแฟ้มที่[อัปโหลด](https://support.office.com/article/Upload-a-folder-or-files-to-a-document-library-eb18fcba-c953-4d45-8d90-8da66edeacdb)[ดาวน์โหลด](https://support.office.com/article/Download-files-and-folders-from-OneDrive-or-SharePoint-5c7397b7-19c7-4893-84fe-d02e8fa5df05)แฟ้ม แฟ้ม[แก้ไข](https://support.office.com/article/Edit-a-document-in-a-document-library-02d8497f-1c13-4114-949a-b8466f639b07)และปัจจุบัน[ข้อจำกัดของแฟ้ม](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa?ui=en-US&amp;rs=en-US&amp;ad=US)</span><span class="sxs-lookup"><span data-stu-id="eca08-108">**Working with Document Files**: Learn more about file [upload](https://support.office.com/article/Upload-a-folder-or-files-to-a-document-library-eb18fcba-c953-4d45-8d90-8da66edeacdb), file [download](https://support.office.com/article/Download-files-and-folders-from-OneDrive-or-SharePoint-5c7397b7-19c7-4893-84fe-d02e8fa5df05), file [edits](https://support.office.com/article/Edit-a-document-in-a-document-library-02d8497f-1c13-4114-949a-b8466f639b07), and current [file limitations](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa?ui=en-US&amp;rs=en-US&amp;ad=US)</span></span>

- <span data-ttu-id="eca08-109">**เก็บข้อมูล**: การเรียนรู้วิธีจัดการการเก็บข้อมูลผู้ใช้ OneDrive</a>เช่น[การจัดการการจัดเก็บของไซต์](https://docs.microsoft.com/sharepoint/manage-site-collection-storage-limits)สำหรับการบอกรับเป็นสมาชิกและ[การทำความเข้าใจเกี่ยวกับข้อจำกัดทั้งหมด](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)</span><span class="sxs-lookup"><span data-stu-id="eca08-109">**Storage**: Learn how to manage your users OneDrive storage</a>, such as [managing site storage](https://docs.microsoft.com/sharepoint/manage-site-collection-storage-limits) for your subscription and [understanding all limits](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits).</span></span>

- <span data-ttu-id="eca08-110">**เปลี่ยนชื่อผู้เช่า**: เห็นการ[เปลี่ยนแปลงชื่อโดเมนของ SharePoint](https://docs.microsoft.com/sharepoint/change-your-sharepoint-domain-name)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="eca08-110">**Tenant Rename**: See [Change your SharePoint domain name](https://docs.microsoft.com/sharepoint/change-your-sharepoint-domain-name) for more information.</span></span>

- <span data-ttu-id="eca08-111">**Modernize SharePoint**: ทบทวน[คำแนะนำกับประสบการณ์ใช้งานแบบสมัยใหม่ใน SharePoint](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience)และ[ไซต์ SharePoint ของคุณแบบคลาสสิ Modernize](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites)เพื่อเริ่มต้นการย้าย</span><span class="sxs-lookup"><span data-stu-id="eca08-111">**Modernize SharePoint**: Review the [Guide to the Modern experience in SharePoint](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience) and [Modernize your classic SharePoint sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites) to start the move.</span></span>

- <span data-ttu-id="eca08-112">**เริ่มต้น**: เรียนรู้วิธีการ[เริ่มต้นใช้งาน SharePoint แบบออนไลน์](https://docs.microsoft.com/sharepoint/introduction)ด้วยกลยุทธ์การจัดการของไซต์</span><span class="sxs-lookup"><span data-stu-id="eca08-112">**Getting Started**: Learn how to [get started with SharePoint Online](https://docs.microsoft.com/sharepoint/introduction) with site management strategies.</span></span>