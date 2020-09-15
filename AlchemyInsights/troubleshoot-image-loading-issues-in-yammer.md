---
title: การแก้ไขปัญหาการโหลดรูปภาพใน Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690262"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="17a7f-102">การแก้ไขปัญหาการโหลดรูปภาพใน Yammer</span><span class="sxs-lookup"><span data-stu-id="17a7f-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="17a7f-103">เมื่อปัญหาเกิดขึ้นกับรูปถ่ายและการแสดงตัวอย่างไฟล์ใน Yammer การแก้ไขปัญหาโดยการตรวจสอบว่าปัญหานี้เกิดขึ้นสำหรับผู้ใช้ทั้งหมดหรือไม่ไม่ว่าจะเกิดปัญหาในอุปกรณ์เคลื่อนที่และถ้าการอัปโหลดสิ่งที่แนบมา</span><span class="sxs-lookup"><span data-stu-id="17a7f-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="17a7f-104">**ปัญหารูปถ่ายของโพรไฟล์**</span><span class="sxs-lookup"><span data-stu-id="17a7f-104">**Profile photo issues**</span></span>  

<span data-ttu-id="17a7f-105">ถ้าผู้ใช้ลงชื่อเข้าใช้ Yammer ผ่าน Microsoft ๓๖๕ผู้ใช้จะต้องเปลี่ยนโปรไฟล์ของพวกเขารวมถึงรูปภาพโปรไฟล์ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="17a7f-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="17a7f-106">ถ้าผู้ใช้ไม่ได้รับอนุญาตให้ทำการอัปเดตโปรไฟล์ผู้ดูแลระบบสามารถทำการอัปเดตสำหรับผู้ใช้ได้</span><span class="sxs-lookup"><span data-stu-id="17a7f-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="17a7f-107">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)</span><span class="sxs-lookup"><span data-stu-id="17a7f-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="17a7f-108">สำหรับข้อมูลเกี่ยวกับการแก้ไขส่วนกำหนดค่ารวมถึงรูปถ่ายโปรไฟล์ให้ดูที่[เปลี่ยนโปรไฟล์ Yammer และการตั้งค่าของฉัน](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)</span><span class="sxs-lookup"><span data-stu-id="17a7f-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="17a7f-109">รูปถ่ายโปรไฟล์ที่อัปเดตจะซิงค์แตกต่างจากแอตทริบิวต์โปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="17a7f-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="17a7f-110">ผู้ใช้ต้องลงชื่อเข้าใช้เพื่อเริ่มการซิงค์รูปถ่ายโปรไฟล์ของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="17a7f-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="17a7f-111">สำหรับข้อมูลให้ดู[ที่รูปภาพโปรไฟล์ผู้ใช้ได้รับการอัปเดตจาก Office ๓๖๕ไปยัง Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)</span><span class="sxs-lookup"><span data-stu-id="17a7f-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="17a7f-112">สำหรับข้อมูลเกี่ยวกับวงจรการใช้งานของผู้ใช้สำหรับ Yammer ให้ดูที่[จัดการผู้ใช้ Yammer ในวงจรชีวิตของพวกเขาจาก Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="17a7f-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="17a7f-113">สำหรับรายละเอียดเกี่ยวกับวิธีการซิงค์รูปภาพโปรไฟล์ทำงานใน Microsoft ๓๖๕ให้ดูที่[ข้อมูลเกี่ยวกับการซิงโครไนซ์รูปภาพโปรไฟล์ใน microsoft ๓๖๕](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)</span><span class="sxs-lookup"><span data-stu-id="17a7f-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="17a7f-114">**การแสดงตัวอย่างเอกสารและปัญหารูปขนาดย่อของรูป**</span><span class="sxs-lookup"><span data-stu-id="17a7f-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="17a7f-115">เมื่อมีการโพสต์ไฟล์หรือรูปภาพไปยัง Yammer การแสดงตัวอย่างอาจไม่ปรากฏขึ้นเนื่องจาก:</span><span class="sxs-lookup"><span data-stu-id="17a7f-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="17a7f-116">ไฟล์เสียหายและไม่สามารถประมวลผลได้</span><span class="sxs-lookup"><span data-stu-id="17a7f-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="17a7f-117">ไฟล์นี้ยังไม่ได้รับการอัปโหลดไปยัง SharePoint Online หรือ Yammer มี metadata ที่ไม่ถูกต้องสำหรับเหตุผลอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="17a7f-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="17a7f-118">Url ที่จำเป็นสำหรับการโหลดรูปภาพตัวอย่างจะถูกบล็อก</span><span class="sxs-lookup"><span data-stu-id="17a7f-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="17a7f-119">การแสดงตัวอย่างไฟล์ถูกเอาออกโดยผู้ใช้ก่อนที่จะลงรายการบัญชี</span><span class="sxs-lookup"><span data-stu-id="17a7f-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="17a7f-120">ปัญหาของบริการที่ทำให้การแสดงตัวอย่างถูกสร้างขึ้น</span><span class="sxs-lookup"><span data-stu-id="17a7f-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="17a7f-121">**หมายเหตุ:** การแสดงตัวอย่างสำหรับลิงก์และการอัปโหลดไฟล์อาจทำงานแตกต่างกัน</span><span class="sxs-lookup"><span data-stu-id="17a7f-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="17a7f-122">ลิงก์ไปยังไฟล์บนอินเทอร์เน็ตหรือลิงก์ที่จำเป็นต้องมีการรับรองความถูกต้องเพิ่มเติมอาจแสดงไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="17a7f-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="17a7f-123">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่แนบไฟล์หรือรูปภาพไปยังข้อความ Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)</span><span class="sxs-lookup"><span data-stu-id="17a7f-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 