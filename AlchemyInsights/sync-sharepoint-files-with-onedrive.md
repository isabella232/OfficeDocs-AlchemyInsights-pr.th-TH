---
title: การแก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737324"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="402f6-102">การแก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="402f6-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="402f6-103">เราขอแนะนำให้ [ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) ที่มี [ไฟล์ตามความต้อง](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) การเนื่องจากมีการเข้าถึงไฟล์ของคุณภายในเครื่องของคุณและมีประสิทธิภาพการทำงานที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="402f6-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="402f6-104">เมื่อต้องการแก้ไขปัญหาการเปิดด้วย Explorer ให้ทำตามขั้นตอนและแนวทางปฏิบัติที่ดีที่สุดในบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="402f6-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="402f6-105">วิธีใช้คำสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="402f6-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="402f6-106">คัดลอกหรือย้ายไฟล์ไลบรารีโดยใช้เปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="402f6-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="402f6-107">**บันทึกย่อ**</span><span class="sxs-lookup"><span data-stu-id="402f6-107">**Note:**</span></span>
>- <span data-ttu-id="402f6-108">เปิดด้วย Explorer เท่านั้นที่ได้รับการสนับสนุนใน Internet Explorer 10 หรือ11</span><span class="sxs-lookup"><span data-stu-id="402f6-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="402f6-109">เปิดด้วย Explorer ไม่ทำงานใน Windows ด้วย Microsoft Edge, Google Chrome, Mozilla Firefox หรือบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="402f6-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="402f6-110">เนื่องจากสาเหตุนี้ตัวเลือกมุมมอง Explorer อาจเป็นสีเทา</span><span class="sxs-lookup"><span data-stu-id="402f6-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="402f6-111">ปุ่มเปิดด้วย Explorer ไม่ปรากฏในประสบการณ์การใช้งานไลบรารีใหม่</span><span class="sxs-lookup"><span data-stu-id="402f6-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="402f6-112">เลือกเมนูดรอปดาวน์**มุมมอง**ที่มุมขวาบน (ชื่อของการเปลี่ยนแปลงแบบหล่นลงทั้งนี้ขึ้นอยู่กับมุมมองปัจจุบันของคุณ) จากนั้นเลือก**ดูใน File Explorer**</span><span class="sxs-lookup"><span data-stu-id="402f6-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
