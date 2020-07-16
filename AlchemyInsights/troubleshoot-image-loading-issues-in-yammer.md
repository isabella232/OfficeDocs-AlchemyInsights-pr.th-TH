---
title: แก้ไขปัญหาการโหลดรูปใน Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148418"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="cb6f4-102">แก้ไขปัญหาการโหลดรูปใน Yammer</span><span class="sxs-lookup"><span data-stu-id="cb6f4-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="cb6f4-103">เมื่อเกิดปัญหากับรูปถ่ายและแสดงตัวอย่างแฟ้มใน Yammer แก้ไขปัญหา โดยตรวจสอบว่า ปัญหาที่เกิดขึ้นสําหรับผู้ใช้ทั้งหมด ไม่ว่าจะเป็นบนอุปกรณ์มือถือ และถ้าเป็น reproducible เมื่ออัปโหลดสิ่งที่แนบ</span><span class="sxs-lookup"><span data-stu-id="cb6f4-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="cb6f4-104">**ปัญหารูปภาพโปรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="cb6f4-104">**Profile photo issues**</span></span>  

<span data-ttu-id="cb6f4-105">ถ้าผู้ใช้ลงชื่อเข้าใช้ Yammer ผ่าน Microsoft 365 ผู้ใช้เหล่านั้นต้องเปลี่ยนโปรไฟล์รวมถึงรูปโปรไฟล์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="cb6f4-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="cb6f4-106">หากผู้ใช้ไม่ได้รับอนุญาตให้อัปเดตโปรไฟล์ผู้ดูแลระบบสามารถทําการอัปเดตสําหรับผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="cb6f4-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="cb6f4-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="cb6f4-108">สําหรับข้อมูลเกี่ยวกับการแก้ไขโปรไฟล์ รวมถึงรูปโปรไฟล์ ให้ดูที่[การเปลี่ยนโปรไฟล์ Yammer และการตั้งค่าของฉัน](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="cb6f4-109">รูปภาพโปรไฟล์ที่อัปเดตจะซิงค์แตกต่างจากคุณลักษณะโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="cb6f4-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="cb6f4-110">ผู้ใช้ต้องลงชื่อเข้าใช้เพื่อเริ่มต้นการซิงค์รูปโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="cb6f4-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="cb6f4-111">สําหรับข้อมูล[ให้ดูที่ รูปภาพโปรไฟล์ผู้ใช้ที่ได้รับการปรับปรุงจาก Office 365 ไปยัง Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="cb6f4-112">สําหรับข้อมูลเกี่ยวกับวงจรการใช้งานของผู้ใช้สําหรับ Yammer ให้ดูที่[จัดการผู้ใช้ Yammer ในวงจรการใช้งานของผู้ใช้จาก Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="cb6f4-113">สําหรับรายละเอียดเกี่ยวกับวิธีการทํางานของการซิงค์รูปภาพโปรไฟล์ใน Microsoft 365 ให้ดูที่[ข้อมูลเกี่ยวกับการทําข้อมูลโปรไฟล์รูปภาพให้ตรงกันใน Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="cb6f4-114">**ตัวอย่างเอกสารและปัญหารูปขนาดย่อของภาพ**</span><span class="sxs-lookup"><span data-stu-id="cb6f4-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="cb6f4-115">เมื่อไฟล์หรือรูปภาพถูกโพสต์ไปยัง Yammer การแสดงตัวอย่างอาจไม่ปรากฏขึ้นเนื่องจาก:</span><span class="sxs-lookup"><span data-stu-id="cb6f4-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="cb6f4-116">แฟ้มเสียหายและไม่สามารถประมวลผลได้</span><span class="sxs-lookup"><span data-stu-id="cb6f4-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="cb6f4-117">แฟ้มไม่ได้ถูกอัปโหลดเมื่อเร็ว ๆ นี้ไปยัง SharePoint แบบออนไลน์ หรือ Yammer มีข้อมูลเมตาที่ไม่ถูกต้องสําหรับเหตุผลอื่น ๆ</span><span class="sxs-lookup"><span data-stu-id="cb6f4-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="cb6f4-118">URL ที่จําเป็นสําหรับการโหลดภาพตัวอย่างจะถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="cb6f4-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="cb6f4-119">การแสดงตัวอย่างไฟล์ถูกลบโดยผู้ใช้ก่อนที่จะลงรายการบัญชี</span><span class="sxs-lookup"><span data-stu-id="cb6f4-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="cb6f4-120">ปัญหาการบริการทําให้การแสดงตัวอย่างถูกสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="cb6f4-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="cb6f4-121">**หมายเหตุ** ตัวอย่างลิงก์และอัปโหลดไฟล์อาจทํางานแตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="cb6f4-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="cb6f4-122">ลิงก์ไปยังแฟ้มบนอินเทอร์เน็ตหรือการเชื่อมโยงที่จําเป็นต้องมีการรับรองความถูกต้องเพิ่มเติมอาจแสดงไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="cb6f4-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="cb6f4-123">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การแนบไฟล์หรือรูปภาพลงในข้อความ Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)</span><span class="sxs-lookup"><span data-stu-id="cb6f4-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 