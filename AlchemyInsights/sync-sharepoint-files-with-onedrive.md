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
ms.openlocfilehash: afee367e250357b20b77f0ea5dfe66d68967eb2a
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270727"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="35310-102">แก้ไขปัญหา "เปิดด้วย Explorer" ใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="35310-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="35310-103">เปิด ด้วยคำสั่ง Explorer เปิดอินสแตนซ์ที่ท้องถิ่นของ Windows Explorer ที่แสดงโครงสร้างของโฟลเดอร์บนเซิร์ฟเวอร์ที่โฮสต์ ไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="35310-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="35310-104">ซึ่งกำลังพูด เราขอแนะนำ[ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>ซึ่งเป็น[แฟ้มตามความต้องการ](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)เนื่องจากมีท้องถิ่นในการเข้าถึงแฟ้มของคุณ และมีประสิทธิภาพที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="35310-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="35310-105">ถ้าคุณเลือกที่จะใช้มุมมอง Explorer แทนการใช้ไคลเอ็นต์การซิงค์ OneDrive ใหม่ ทำให้แน่ใจว่า คุณทำตามขั้นตอนและวิธีปฏิบัติที่ดีที่สุดในบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="35310-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="35310-106">วิธีการใช้คำสั่ง "เปิดด้วย Explorer" การแก้ไขปัญหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="35310-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="35310-107">คัดลอก หรือย้ายแฟ้มไลบรารี โดยใช้เปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="35310-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="35310-108">ปุ่ม**เปิด ด้วย Explorer**ไม่ปรากฏขึ้นในประสบการณ์ใช้งานของไลบรารีใหม่</span><span class="sxs-lookup"><span data-stu-id="35310-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="35310-109">เลือกมุม**มอง**แบบหล่นลงในมุมบนขวา (ชื่อของการเปลี่ยนแปลงแบบหล่นลงโดยขึ้นอยู่กับมุมมองปัจจุบันของคุณ), และจากนั้น เลือก**มุมมองใน Explorer แฟ้ม**</span><span class="sxs-lookup"><span data-stu-id="35310-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="35310-110">เปิด SharePoint ด้วย Explorer ใช้ตัวควบคุม ActiveX ดังนั้นเท่านั้นได้รับการสนับสนุนใน Internet Explorer 10 หรือ 11</span><span class="sxs-lookup"><span data-stu-id="35310-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="35310-111">เปิด ด้วย Explorer ไม่ทำงานใน Windows ด้วยขอบ Microsoft โครเมียม Google, Mozilla Firefox หรือ บนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="35310-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="35310-112">เนื่องจากสาเหตุนี้ ตัวเลือกมุมมอง Explorer อาจเป็นสีเทา</span><span class="sxs-lookup"><span data-stu-id="35310-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="35310-113">[ปุ่ม ribbon เหตุ SharePoint จะไม่พร้อมใช้งาน หรือสีเทา](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="35310-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

