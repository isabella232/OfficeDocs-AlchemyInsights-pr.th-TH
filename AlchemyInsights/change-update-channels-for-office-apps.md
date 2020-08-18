---
title: เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786872"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="3c30a-102">เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office</span><span class="sxs-lookup"><span data-stu-id="3c30a-102">Change update channels for Office apps</span></span>

<span data-ttu-id="3c30a-103">สำหรับการติดตั้ง Office ใหม่ให้ใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ของ Office เพื่อเลือกแชนเนลการอัปเดตที่ต้องการจากนั้นติดตั้ง (หรือติดตั้งใหม่) แอป Office</span><span class="sxs-lookup"><span data-stu-id="3c30a-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="3c30a-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการการตั้งค่าการดาวน์โหลดซอฟต์แวร์ใน Office ๓๖๕](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)</span><span class="sxs-lookup"><span data-stu-id="3c30a-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="3c30a-105">**หมายเหตุ:** ช่องทางการอัปเดตที่เลือกโดยใช้การตั้งค่าการดาวน์โหลดซอฟต์แวร์ของ Office จะนำไปใช้กับผู้ใช้ทุกคนที่ทำการติดตั้งใหม่โดยใช้ O365 portal</span><span class="sxs-lookup"><span data-stu-id="3c30a-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="3c30a-106">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ดาวน์โหลดและติดตั้งหรือติดตั้ง Microsoft ๓๖๕หรือ Office ๒๐๑๙อีกครั้งบนพีซีหรือ Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)</span><span class="sxs-lookup"><span data-stu-id="3c30a-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="3c30a-107">สำหรับการติดตั้ง Office ที่มีอยู่ให้ใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อสลับไปยังแชนเนลการอัปเดตที่แตกต่างกันดังนี้</span><span class="sxs-lookup"><span data-stu-id="3c30a-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="3c30a-108">ดาวน์โหลดเวอร์ชันล่าสุดของเครื่องมือการปรับใช้ Office (setup.exe) จาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="3c30a-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="3c30a-109">ระบุชื่อของแชนเนลที่คุณต้องการสลับไปใช้</span><span class="sxs-lookup"><span data-stu-id="3c30a-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="3c30a-110">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตัวเลือกการกำหนดค่าสำหรับเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)</span><span class="sxs-lookup"><span data-stu-id="3c30a-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="3c30a-111">สร้างไฟล์ XML การกำหนดค่าที่ระบุชื่อแชนเนลที่เหมาะสมตัวอย่างเช่น update.xml</span><span class="sxs-lookup"><span data-stu-id="3c30a-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="3c30a-112">จากพร้อมท์คำสั่งยกระดับให้สลับไปยังตำแหน่งที่ตั้งของโฟลเดอร์ที่ setup.exe อยู่และเรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3c30a-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="3c30a-113">a.</span><span class="sxs-lookup"><span data-stu-id="3c30a-113">a.</span></span> <span data-ttu-id="3c30a-114">setup.exe c:\odt\setup.exe/configure update.xml</span><span class="sxs-lookup"><span data-stu-id="3c30a-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="3c30a-115">เริ่มแอปพลิเคชัน Office (เช่น Excel) แล้วเลือก**File**  >  **บัญชีผู้ใช้**ไฟล์</span><span class="sxs-lookup"><span data-stu-id="3c30a-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="3c30a-116">ในส่วนข้อมูลผลิตภัณฑ์ให้เลือกอัปเดตตัว**เลือกการอัปเด**  >  **ตเดี๋ยวนี้**</span><span class="sxs-lookup"><span data-stu-id="3c30a-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="3c30a-117">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการสลับช่องทางการอัปเดตสำหรับแอป Office ที่มีอยู่](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)</span><span class="sxs-lookup"><span data-stu-id="3c30a-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="3c30a-118">สำหรับการสลับช่องทางการอัปเดตสำหรับกลุ่มผู้ใช้ที่เลือกหรือโดยการใช้ตัวจัดการการตั้งค่าคอนฟิก (SCCM) ให้กำหนดค่าการตั้งค่าการอัปเดตระเบียนโดยใช้วัตถุนโยบายกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="3c30a-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="3c30a-119">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ภาพรวมของช่องทางการอัปเดตสำหรับแอป Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)</span><span class="sxs-lookup"><span data-stu-id="3c30a-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="3c30a-120">สำหรับรายละเอียดให้ดู [ที่วิธีการจัดการ Office ๓๖๕ ProPlus channel สำหรับผู้เชี่ยวชาญด้าน it](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) และ [จัดการการอัปเดตเป็นแอป Microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า microsoft จุดสิ้น](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)สุด</span><span class="sxs-lookup"><span data-stu-id="3c30a-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>