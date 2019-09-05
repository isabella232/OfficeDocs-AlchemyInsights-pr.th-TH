---
title: แก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint แบบออนไลน์
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 73583b3b27143c708a4cc993cdff94a33131ab52
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36743112"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b968b-102">แก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="b968b-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="b968b-103">คำสั่ง Open ด้วย Explorer เปิดอินสแตนซ์ภายในเครื่องของ Windows Explorer ที่แสดงโครงสร้างของโฟลเดอร์บนเซิร์ฟเวอร์ที่โฮสต์ไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="b968b-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="b968b-104">นี้ถูกกล่าวว่าเราขอแนะนำให้</a> [ซิงค์แฟ้ม SharePoint กับไคลเอ็นต์ซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)ซึ่งมี[แฟ้มตามความต้อง](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)การเนื่องจากมีการเข้าถึงภายในเครื่องไปยังแฟ้มของคุณและมีประสิทธิภาพการทำงานที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="b968b-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="b968b-105">ถ้าคุณเลือกที่จะใช้มุมมอง Explorer แทนที่จะใช้ไคลเอ็นต์การซิงค์ OneDrive ใหม่ให้แน่ใจว่าคุณทำตามขั้นตอนและแนวทางปฏิบัติที่ดีที่สุดในบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b968b-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b968b-106">วิธีการใช้คำสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="b968b-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="b968b-107">คัดลอกหรือย้ายแฟ้มไลบรารีโดยใช้เปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="b968b-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="b968b-108">ปุ่ม**เปิดด้วย Explorer**จะไม่ปรากฏในประสบการณ์ใช้งานไลบรารีใหม่</span><span class="sxs-lookup"><span data-stu-id="b968b-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b968b-109">เลือก**มุมมอง**แบบหล่นลงที่ด้านบนขวา (ชื่อของการเปลี่ยนแปลงแบบหล่นลงขึ้นอยู่กับมุมมองปัจจุบันของคุณ), และจากนั้นเลือก**มุมมองในแฟ้ม Explorer**</span><span class="sxs-lookup"><span data-stu-id="b968b-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="b968b-110">SharePoint เปิดด้วย Explorer ใช้ตัวควบคุม ActiveX ดังนั้นจึงได้รับการสนับสนุนใน Internet Explorer 10 หรือ11เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="b968b-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b968b-111">เปิดด้วย Explorer ไม่ทำงานใน Windows ด้วย Microsoft Edge, Google โครเมียม, Mozilla Firefox หรือบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="b968b-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b968b-112">ด้วยเหตุนี้ตัวเลือกมุมมอง Explorer อาจเป็นสีเทา</span><span class="sxs-lookup"><span data-stu-id="b968b-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="b968b-113">[ทำไมปุ่ม ribbon ของ SharePoint จึงไม่พร้อมใช้งานหรือเป็นสีเทา](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="b968b-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

