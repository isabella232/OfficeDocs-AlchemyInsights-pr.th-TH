---
title: ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757838"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="97d6a-102">ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่</span><span class="sxs-lookup"><span data-stu-id="97d6a-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="97d6a-103">เปิด ด้วยคำสั่ง Explorer เปิดอินสแตนซ์ที่ท้องถิ่นของ Windows Explorer ที่แสดงโครงสร้างของโฟลเดอร์บนเซิร์ฟเวอร์ที่โฮสต์ ไซต์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="97d6a-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="97d6a-104">ซึ่งกำลังพูด เราขอแนะนำ[ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>ซึ่งเป็น[แฟ้มตามความต้องการ](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)เนื่องจากมีท้องถิ่นในการเข้าถึงแฟ้มของคุณ และมีประสิทธิภาพที่ดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="97d6a-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="97d6a-105">ถ้าคุณเลือกที่จะใช้มุมมอง explorer แทนการใช้ไคลเอนต์ซิงค์ใหม่ ให้แน่ใจว่า คุณทำตามขั้นตอนและวิธีปฏิบัติที่ดีที่สุดในบทความ</span><span class="sxs-lookup"><span data-stu-id="97d6a-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="97d6a-106">วิธีการใช้คำสั่ง "เปิดด้วย Explorer" การแก้ไขปัญหาใน SharePoint แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="97d6a-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="97d6a-107">คัดลอก หรือย้ายแฟ้มไลบรารี โดยใช้เปิดด้วย Explorer</span><span class="sxs-lookup"><span data-stu-id="97d6a-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="97d6a-108">หมายเหตุ: เปิด ด้วย Explorer ปุ่มไม่ปรากฏอยู่ในประสบการณ์ใช้งานของไลบรารีใหม่</span><span class="sxs-lookup"><span data-stu-id="97d6a-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="97d6a-109">คลิกมุมมองแบบหล่นลงในมุมขวาด้านบน (ชื่อของการเปลี่ยนแปลงแบบหล่นลงโดยขึ้นอยู่กับมุมมองปัจจุบันของคุณ), และจากนั้น คลิกมุมมองใน Explorer แฟ้ม</span><span class="sxs-lookup"><span data-stu-id="97d6a-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="97d6a-110">เปิด SharePoint ด้วย Explorer ใช้ตัวควบคุม ActiveX ดังนั้นเท่านั้นได้รับการสนับสนุนใน Internet Explorer 10 หรือ 11</span><span class="sxs-lookup"><span data-stu-id="97d6a-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="97d6a-111">เปิด ด้วย Explorer ไม่ทำงานใน Windows ด้วยขอบ Microsoft โครเมียม Google, Mozilla Firefox หรือ บนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="97d6a-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="97d6a-112">เนื่องจากสาเหตุนี้ ตัวเลือกมุมมอง Explorer อาจเป็นสีเทา</span><span class="sxs-lookup"><span data-stu-id="97d6a-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="97d6a-113">[ปุ่ม ribbon เหตุ SharePoint จะไม่พร้อมใช้งาน หรือสีเทา](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="97d6a-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

