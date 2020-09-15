---
title: ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695668"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="36fac-102">ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ใน Yammer</span><span class="sxs-lookup"><span data-stu-id="36fac-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="36fac-103">Yammer คลาสสิกสนับสนุนตัวเลือกหลายตัวเลือกสำหรับการอัปโหลดไฟล์ไปยังข้อความและกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="36fac-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="36fac-104">โดยขึ้นอยู่กับการกำหนดค่าเครือข่ายไฟล์ค่าเริ่มต้นไปยังที่เก็บข้อมูลใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="36fac-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="36fac-105">ตัวใช้เลือกไฟล์ใน Yammer ใหม่ยังไม่สนับสนุนตัวเลือกทั้งหมดที่พร้อมใช้งานใน Yammer แบบคลาสสิก</span><span class="sxs-lookup"><span data-stu-id="36fac-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="36fac-106">การอัปเดตในอนาคตจะเพิ่มฟีเจอร์เพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="36fac-106">A future update will add additional features.</span></span> <span data-ttu-id="36fac-107">สำหรับข้อมูลเพิ่มเติมให้ดูที่[แนบไฟล์หรือรูปภาพลงในโพสต์การสนทนา Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)</span><span class="sxs-lookup"><span data-stu-id="36fac-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="36fac-108">**ไม่สามารถเปิดหรือดาวน์โหลดไฟล์ได้**</span><span class="sxs-lookup"><span data-stu-id="36fac-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="36fac-109">ไฟล์อาจอัปโหลดไปยัง Yammer แต่ยังสามารถเชื่อมโยงไปยังไฟล์ใน SharePoint Online ได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="36fac-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="36fac-110">เมื่อต้องการแก้ไขปัญหาก่อนอื่นคุณจะต้องระบุตำแหน่งที่ตั้งของไฟล์นั้น</span><span class="sxs-lookup"><span data-stu-id="36fac-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="36fac-111">ถ้าไฟล์ได้รับการอัปโหลดไปยัง Yammer จะมี URL \* yammer.com</span><span class="sxs-lookup"><span data-stu-id="36fac-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="36fac-112">ตรวจสอบให้แน่ใจว่า Url ที่จำเป็นและที่อยู่ IP ไม่ได้รับการบล็อก</span><span class="sxs-lookup"><span data-stu-id="36fac-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="36fac-113">สำหรับข้อมูลเพิ่มเติมให้ดูที่โพสต์ในบล็อก[โดยใช้ที่อยู่ IP ของรหัสที่ฮาร์สำหรับ Yammer ไม่แนะนำ](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)</span><span class="sxs-lookup"><span data-stu-id="36fac-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="36fac-114">ตรวจสอบว่าผู้ใช้ที่เป็นผู้ดูแลระบบส่วนกลางสามารถดาวน์โหลดไฟล์ได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="36fac-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="36fac-115">ถ้าไฟล์เป็นแบบส่วนตัวคุณอาจจำเป็นต้องใช้โหมดเนื้อหาส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="36fac-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="36fac-116">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตรวจสอบเนื้อหาส่วนตัวใน Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)</span><span class="sxs-lookup"><span data-stu-id="36fac-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="36fac-117">**ผู้เยี่ยมชมระดับเครือข่าย Yammer และไฟล์ใน SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="36fac-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="36fac-118">[ผู้เยี่ยมชมระดับเครือข่ายใน Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ไม่ได้ใช้ AZURE AD B2B และอยู่ภายในบริการ Yammer ดังนั้นจึงไม่สามารถเข้าถึงไฟล์ Yammer ที่เก็บไว้ใน SharePoint ได้</span><span class="sxs-lookup"><span data-stu-id="36fac-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="36fac-119">สร้างผู้ใช้ B2B ภายนอกที่สามารถเข้าถึงไลบรารีเอกสารใน SharePoint Online โดยใช้ข้อมูลประจำตัวนั้น</span><span class="sxs-lookup"><span data-stu-id="36fac-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="36fac-120">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสนับสนุนของผู้เยี่ยมชมในอนาคตของ Azure AD ใน Yammer ให้ดูที่[การสนับสนุนของผู้เข้าร่วมทางธุรกิจ (B2B) ในการแสดงตัวอย่าง Yammer-ข้อกำหนดและคำถามที่ถามบ่อยของลูกค้า](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)</span><span class="sxs-lookup"><span data-stu-id="36fac-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>