---
title: ๒๖๐๙-การเก็บรักษา-หรือ ediscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994102"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="b57ca-102">ไม่สามารถลบรายการใน SharePoint แบบออนไลน์หรือ OneDrive สำหรับธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="b57ca-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="b57ca-103">คุณหรือผู้ใช้ของคุณอาจไม่สามารถลบรายการใน SharePoint แบบออนไลน์หรือ OneDrive สำหรับธุรกิจเนื่องจากนโยบายการเก็บข้อมูล, ป้ายชื่อการเก็บข้อมูลหรือการระงับ eDiscovery ถูกนำไปใช้กับ SharePoint ของไซต์ OneDrive หรือไปยังรายการเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="b57ca-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="b57ca-104">ซึ่งรวมถึงการไม่สามารถลบเอกสารรุ่นเอกสารโฟลเดอร์ไลบรารีเอกสารรายการแอปไซต์หรือชุดเก็บรวบรวมไซต์</span><span class="sxs-lookup"><span data-stu-id="b57ca-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="b57ca-105">ต่อไปนี้เป็นตัวอย่างของข้อผิดพลาดที่คุณอาจได้รับถ้าคุณพยายามที่จะลบรายการที่ถูกเก็บไว้:</span><span class="sxs-lookup"><span data-stu-id="b57ca-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="b57ca-106">"ไซต์นี้ไม่สามารถลบได้เนื่องจากมีการรวมอยู่ในนโยบายการระงับหรือการเก็บข้อมูล eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="b57ca-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="b57ca-107">"ไซต์นี้มีการตั้งค่านโยบายการปฏิบัติตามกฎระเบียบเพื่อบล็อกการลบ"</span><span class="sxs-lookup"><span data-stu-id="b57ca-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="b57ca-108">"นโยบายการปฏิบัติตามกฎระเบียบกำลังบล็อกการลบไซต์นี้อยู่ในขณะนี้"</span><span class="sxs-lookup"><span data-stu-id="b57ca-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="b57ca-109">"ไม่สามารถลบไซต์คอลเลกชันนี้ได้เนื่องจากมีไซต์ที่รวมอยู่ในนโยบายการระงับหรือการเก็บข้อมูล eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="b57ca-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="b57ca-110">"คุณต้องลบรายการทั้งหมดในโฟลเดอร์นี้ก่อนที่จะลบโฟลเดอร์"</span><span class="sxs-lookup"><span data-stu-id="b57ca-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="b57ca-111">"รุ่นของรายการนี้ไม่สามารถลบได้เนื่องจากมีการระงับหรือนโยบายการเก็บข้อมูล"</span><span class="sxs-lookup"><span data-stu-id="b57ca-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="b57ca-112">"ไม่สามารถลบรายการในขณะค้าง"</span><span class="sxs-lookup"><span data-stu-id="b57ca-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="b57ca-113">"ป้ายชื่อที่ใช้กับรายการนี้จะป้องกันไม่ให้มีการแก้ไขหรือลบ"</span><span class="sxs-lookup"><span data-stu-id="b57ca-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="b57ca-114">"รายการไม่สามารถลบได้ในขณะที่มีการระงับหรือนโยบายการเก็บข้อมูล"</span><span class="sxs-lookup"><span data-stu-id="b57ca-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="b57ca-115">"ไม่สามารถลบรายการได้ถ้ามีการบล็อกหรือถ้ามีการใช้นโยบายการเก็บข้อมูลนั้น"</span><span class="sxs-lookup"><span data-stu-id="b57ca-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="b57ca-116">หากต้องการลบรายการต่างๆในสถานการณ์เหล่านี้จะมีการนำนโยบายการเก็บข้อมูลหรือการระงับ eDiscovery ออก (หรือไซต์จะถูกยกเว้นจากนโยบายการเก็บข้อมูล)</span><span class="sxs-lookup"><span data-stu-id="b57ca-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="b57ca-117">คุณจำเป็นต้องปิดใช้งานหรือยกเว้นการระงับที่เกี่ยวข้องซึ่งทำให้เกิดปัญหานี้</span><span class="sxs-lookup"><span data-stu-id="b57ca-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="b57ca-118">หลังจากที่นโยบายการเก็บรักษาหรือการระงับจะถูกลบออกอาจใช้เวลาถึง24ชั่วโมงจึงจะมีผล</span><span class="sxs-lookup"><span data-stu-id="b57ca-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="b57ca-119">สำหรับข้อมูลเกี่ยวกับการเก็บรักษาที่แตกต่างกันและเก็บคุณลักษณะที่สามารถนำไปใช้กับไซต์ SharePoint และบัญชี OneDrive ดูหนึ่งในหัวข้อต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="b57ca-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="b57ca-120">ภาพรวมของนโยบายการเก็บข้อมูล</span><span class="sxs-lookup"><span data-stu-id="b57ca-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="b57ca-121">ภาพรวมของป้ายชื่อการเก็บรักษา</span><span class="sxs-lookup"><span data-stu-id="b57ca-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="b57ca-122">จัดการการระงับใน eDiscovery ขั้นสูง</span><span class="sxs-lookup"><span data-stu-id="b57ca-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="b57ca-123">การระงับ eDiscovery</span><span class="sxs-lookup"><span data-stu-id="b57ca-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="b57ca-124">นโยบายการปิดและการลบไซต์ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="b57ca-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
