---
title: ปัญหาการเปิดหรือดาวน์โหลดแฟ้มใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148436"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="0fca8-102">ปัญหาการเปิดหรือดาวน์โหลดแฟ้มใน Yammer</span><span class="sxs-lookup"><span data-stu-id="0fca8-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="0fca8-103">Yammer แบบคลาสสิกสนับสนุนตัวเลือกหลายตัวเลือกสําหรับการอัปโหลดแฟ้มไปยังข้อความและกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="0fca8-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="0fca8-104">แฟ้มเริ่มต้นสําหรับที่เก็บข้อมูลใน SharePoint ขึ้นอยู่กับการกําหนดค่าเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="0fca8-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="0fca8-105">ตัวเลือกแฟ้มใน Yammer ใหม่ไม่สนับสนุนตัวเลือกทั้งหมดที่มีอยู่ใน Yammer แบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="0fca8-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="0fca8-106">การปรับปรุงในอนาคตจะเพิ่มคุณลักษณะเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="0fca8-106">A future update will add additional features.</span></span> <span data-ttu-id="0fca8-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[แนบไฟล์หรือรูปภาพลงในโพสต์สนทนา Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)</span><span class="sxs-lookup"><span data-stu-id="0fca8-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="0fca8-108">**ไม่สามารถเปิดหรือดาวน์โหลดแฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="0fca8-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="0fca8-109">แฟ้มอาจอัปโหลดไปยัง Yammer แต่ยังเชื่อมโยงไปยังแฟ้มใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="0fca8-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="0fca8-110">เมื่อต้องการแก้ไขปัญหา ก่อนอื่นคุณต้องกําหนดตําแหน่งที่ตั้งของแฟ้ม</span><span class="sxs-lookup"><span data-stu-id="0fca8-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="0fca8-111">ถ้าแฟ้มถูกอัปโหลดไปยัง Yammer แฟ้มนั้นจะมี URL \*.yammer.com</span><span class="sxs-lookup"><span data-stu-id="0fca8-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="0fca8-112">ตรวจสอบให้แน่ใจว่า URL และที่อยู่ IP ที่ต้องการถูกยกเลิกการบล็อก</span><span class="sxs-lookup"><span data-stu-id="0fca8-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="0fca8-113">สําหรับข้อมูลเพิ่มเติม[ให้ดูที่โพสต์บล็อก](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)</span><span class="sxs-lookup"><span data-stu-id="0fca8-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="0fca8-114">ตรวจสอบว่าผู้ใช้ที่เป็นผู้ดูแลระบบส่วนกลางสามารถดาวน์โหลดไฟล์ได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="0fca8-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="0fca8-115">ถ้าแฟ้มเป็นส่วนตัว คุณอาจต้องใช้โหมดเนื้อหาส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="0fca8-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="0fca8-116">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตรวจสอบเนื้อหาส่วนตัวใน Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)</span><span class="sxs-lookup"><span data-stu-id="0fca8-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="0fca8-117">**ผู้ใช้และแฟ้มระดับเครือข่าย Yammer ใน SharePoint แบบออนไลน์**</span><span class="sxs-lookup"><span data-stu-id="0fca8-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="0fca8-118">[ผู้ใช้ระดับเครือข่ายใน Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)ไม่ได้ใช้ Azure AD B2B และภายในไปยังบริการ Yammer ดังนั้นพวกเขาจึงไม่สามารถเข้าถึงแฟ้ม Yammer ที่เก็บไว้ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="0fca8-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="0fca8-119">สร้างผู้ใช้ AAD B2B ภายนอกที่สามารถเข้าถึงไลบรารีเอกสารใน SharePoint แบบออนไลน์ โดยใช้ข้อมูลประจําตัวนั้น</span><span class="sxs-lookup"><span data-stu-id="0fca8-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="0fca8-120">สําหรับข้อมูลเกี่ยวกับการสนับสนุนผู้เยี่ยมชม Azure AD B2B ในอนาคตใน Yammer ให้ดูที่[การสนับสนุนผู้เยี่ยมชมธุรกิจ (B2B) ใน Yammer Preview - ข้อกําหนดของลูกค้าและคําถามที่ถามบ่อย](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)</span><span class="sxs-lookup"><span data-stu-id="0fca8-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>