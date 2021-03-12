---
title: ไม่สามารถเข้าถึงไซต์นี้ - ข้อผิดพลาดเมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747036"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="5e7fb-102">ข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams</span><span class="sxs-lookup"><span data-stu-id="5e7fb-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="5e7fb-103">ผู้ใช้อาจได้รับข้อผิดพลาด "ไม่สามารถเข้าถึงไซต์นี้" เมื่อพยายามเข้าถึงไซต์ SharePoint จากเบราว์เซอร์หรือ Teams</span><span class="sxs-lookup"><span data-stu-id="5e7fb-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="5e7fb-104">เมื่อต้องการแก้ไขปัญหานี้:</span><span class="sxs-lookup"><span data-stu-id="5e7fb-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="5e7fb-105">ตรวจสอบว่าโฮมเพจอยู่ในถังรีไซเคิลหรือถังรีไซเคิลขั้นที่สองและคืนค่าหน้า</span><span class="sxs-lookup"><span data-stu-id="5e7fb-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="5e7fb-106">**ตัวอย่าง URL โดยตรงไปยังถังรีไซเคิล**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="5e7fb-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="5e7fb-107">ถ้าโฮมเพจถูกเอาออกจากถังรีไซเคิลอย่างถาวร ให้สร้างหน้าไซต์ใหม่จากไลบรารีหน้าไซต์แล้วสร้างโฮมเพจ</span><span class="sxs-lookup"><span data-stu-id="5e7fb-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="5e7fb-108">**ตัวอย่าง URL โดยตรง**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="5e7fb-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>