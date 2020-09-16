---
title: ๒๖๐๙-การเก็บข้อมูลหรือการระงับ ediscovery
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727910"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="5f9e1-102">ไม่สามารถลบรายการใน SharePoint Online หรือ OneDrive for Business ได้</span><span class="sxs-lookup"><span data-stu-id="5f9e1-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="5f9e1-103">คุณหรือผู้ใช้ของคุณอาจไม่สามารถลบรายการใน SharePoint Online หรือ OneDrive for Business ได้เนื่องจากนโยบายการเก็บข้อมูลป้ายชื่อการเก็บข้อมูลหรือการระงับ eDiscovery จะถูกนำไปใช้กับ SharePoint ของไซต์ OneDrive หรือไปยังรายการที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="5f9e1-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="5f9e1-104">ซึ่งรวมถึงการไม่สามารถลบเอกสารเวอร์ชันเอกสารโฟลเดอร์ไลบรารีเอกสารรายการแอปไซต์หรือไซต์คอลเลกชันได้</span><span class="sxs-lookup"><span data-stu-id="5f9e1-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="5f9e1-105">เมื่อต้องการลบรายการในสถานการณ์ใดสถานการณ์หนึ่งต่อไปนี้นโยบายการเก็บข้อมูล, ป้ายชื่อการเก็บข้อมูลหรือการระงับ eDiscovery จะถูกเอาออก (หรือไซต์จะถูกแยกออกจากนโยบายการเก็บข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="5f9e1-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="5f9e1-106">คุณจำเป็นต้องปิดใช้งานหรือไม่รวมการระงับที่เกี่ยวข้องที่ทำให้เกิดปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="5f9e1-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5f9e1-107">หลังจากที่นโยบายการเก็บข้อมูลหรือการระงับถูกเอาออกอาจใช้เวลาถึง24ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="5f9e1-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="5f9e1-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับฟีเจอร์การเก็บข้อมูลและการเก็บข้อมูลที่แตกต่างกันที่สามารถนำไปใช้กับไซต์ SharePoint และบัญชี OneDrive ให้ดูที่หัวข้อใดหัวข้อหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="5f9e1-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="5f9e1-109">ภาพรวมของนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="5f9e1-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="5f9e1-110">ภาพรวมของป้ายชื่อการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="5f9e1-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="5f9e1-111">การจัดการที่ถือใน eDiscovery ขั้นสูง</span><span class="sxs-lookup"><span data-stu-id="5f9e1-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="5f9e1-112">eDiscovery จะถือ</span><span class="sxs-lookup"><span data-stu-id="5f9e1-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="5f9e1-113">นโยบายการปิดและการลบไซต์ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="5f9e1-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)