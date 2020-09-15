---
title: การกำหนดเวอร์ชันใน SharePoint และ OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 12207efc9822be6cf096fa4884a3cd244a286cbe
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653748"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="91b57-102">การกำหนดเวอร์ชันใน SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="91b57-102">Versioning in SharePoint and OneDrive</span></span> 


<span data-ttu-id="91b57-103">เมื่อเปิดใช้งานการกำหนดเวอร์ชันในรายการหรือไลบรารี SharePoint ของคุณคุณสามารถจัดเก็บติดตามและคืนค่ารายการในรายการและไฟล์ในไลบรารีได้เมื่อใดก็ตามที่มีการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="91b57-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="91b57-104">การกำหนดเวอร์ชันที่รวมเข้ากับการตั้งค่าอื่นๆเช่นเช็คเอาท์จะทำให้คุณสามารถควบคุมเนื้อหาที่โพสต์บนไซต์ของคุณได้มากและสามารถระบุค่าจริงได้ถ้าคุณต้องการดูหรือคืนค่าเวอร์ชันเก่าของรายการหรือไฟล์</span><span class="sxs-lookup"><span data-stu-id="91b57-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="91b57-105">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดเวอร์ชันโปรดเยี่ยมชมบทความด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="91b57-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="91b57-106">การกำหนดเวอร์ชันทำงานอย่างไรในรายการหรือไลบรารี SharePoint</span><span class="sxs-lookup"><span data-stu-id="91b57-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="91b57-107">การเปิดใช้งานและกำหนดค่าการกำหนดเวอร์ชันสำหรับรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="91b57-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f)

- [<span data-ttu-id="91b57-108">วิธีการดูประวัติเวอร์ชัน</span><span class="sxs-lookup"><span data-stu-id="91b57-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="91b57-109">คืนค่าไฟล์เวอร์ชันก่อนหน้าใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="91b57-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893)

- [<span data-ttu-id="91b57-110">ดูไฟล์ Office เวอร์ชันก่อนหน้า</span><span class="sxs-lookup"><span data-stu-id="91b57-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="91b57-111">ขีดจำกัดการกำหนดเวอร์ชัน</span><span class="sxs-lookup"><span data-stu-id="91b57-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="91b57-112">ถ้าคุณเป็นลูกค้า Microsoft ๓๖๕การกำหนดเวอร์ชันจะเปิดใช้งานตามค่าเริ่มต้นเมื่อคุณสร้างไลบรารี OneDrive for Business ใหม่และจะบันทึกเวอร์ชัน๕๐๐ของเอกสารล่าสุดโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="91b57-112">If you are a Microsoft 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="91b57-113">การทำเช่นนี้จะช่วยให้คุณป้องกันไม่ให้เอกสารหรือข้อมูลที่สำคัญสูญหาย</span><span class="sxs-lookup"><span data-stu-id="91b57-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="91b57-114">ถ้าคุณมีไลบรารีที่มีอยู่บนไซต์ OneDrive for Business ของคุณหรือบนไซต์ทีมของคุณที่ไม่ได้เปิดใช้งานการกำหนดเวอร์ชันคุณสามารถเปิดใช้งานการกำหนดเวอร์ชันสำหรับพวกเขาได้ตลอดเวลา</span><span class="sxs-lookup"><span data-stu-id="91b57-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


