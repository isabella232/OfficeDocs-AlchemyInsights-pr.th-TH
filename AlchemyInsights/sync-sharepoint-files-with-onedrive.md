---
title: แก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint แบบออนไลน์
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 2023593e281170cea0b055c54d18ef307c4c7ea7
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "43767052"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="ac1f4-102">แก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ac1f4-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="ac1f4-103">เราขอแนะนําให้[ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ซึ่งให้[ไฟล์แบบตามต้องการ](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)เนื่องจากให้การเข้าถึงไฟล์ของคุณภายในเครื่องและนําเสนอประสิทธิภาพที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="ac1f4-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="ac1f4-104">เมื่อต้องการแก้ไขปัญหาเปิดด้วย Explorer ให้ทําตามขั้นตอนและแนวทางปฏิบัติที่ดีที่สุดในบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ac1f4-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="ac1f4-105">วิธีการใช้คําสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="ac1f4-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="ac1f4-106">คัดลอกหรือย้ายแฟ้มไลบรารีโดยใช้เปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="ac1f4-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="ac1f4-107">**หมาย เหตุ:**</span><span class="sxs-lookup"><span data-stu-id="ac1f4-107">**Note:**</span></span>
>
>- <span data-ttu-id="ac1f4-108">ปุ่ม เปิดด้วย Explorer ไม่ปรากฏในประสบการณ์การใช้งานไลบรารีใหม่</span><span class="sxs-lookup"><span data-stu-id="ac1f4-108">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="ac1f4-109">เลือกแบบดรอปดาวน์ **"มุมมอง**" ที่ด้านขวาบน (ชื่อของการเปลี่ยนแปลงแบบดรอปดาวน์ขึ้นอยู่กับมุมมองปัจจุบันของคุณ) แล้วเลือก**View in File Explorer**</span><span class="sxs-lookup"><span data-stu-id="ac1f4-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
>- <span data-ttu-id="ac1f4-110">เปิดด้วย Explorer เท่านั้นได้รับการสนับสนุนใน Internet Explorer 10 หรือ 11</span><span class="sxs-lookup"><span data-stu-id="ac1f4-110">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="ac1f4-111">เปิดด้วย Explorer ไม่ได้ทํางานใน Windows กับไมโครซอฟท์ขอบ, Google Chrome, Mozilla Firefox หรือบนแพลตฟอร์ม Mac.</span><span class="sxs-lookup"><span data-stu-id="ac1f4-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="ac1f4-112">เนื่องจากเหตุผลนี้ Explorer มุมมองตัวเลือกอาจเป็นสีเทา</span><span class="sxs-lookup"><span data-stu-id="ac1f4-112">Due to this reason, the Explorer View option may be grayed out.</span></span>


