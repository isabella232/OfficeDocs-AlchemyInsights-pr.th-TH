---
title: ควบคุมการอัปเดตอัตโนมัติสำหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747795"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="e9f21-102">ควบคุมการอัปเดตอัตโนมัติสำหรับแอป Office</span><span class="sxs-lookup"><span data-stu-id="e9f21-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="e9f21-103">ตามค่าเริ่มต้นการอัปเดตสำหรับแอป Office จะได้รับการดาวน์โหลดโดยอัตโนมัติและนำไปใช้ในพื้นหลังโดยไม่มีการขัดจังหวะของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e9f21-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="e9f21-104">อย่างไรก็ตามผู้ดูแลระบบสามารถควบคุมวิธีการนำการอัปเดตไปใช้ได้โดยใช้การตั้งค่าการอัปเดต Office</span><span class="sxs-lookup"><span data-stu-id="e9f21-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="e9f21-105">อัปเดตการตั้งค่าอนุญาตให้ผู้ดูแลระบบเปิดใช้งานหรือปิดใช้งานการอัปเดตอัตโนมัติแสดงหรือซ่อนปุ่ม **อัปเด** ตทันทีใน Office ตั้งค่ากำหนดเวลาสิ้นสุดการอัปเดตและอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="e9f21-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="e9f21-106">สำหรับข้อมูลโดยละเอียดให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="e9f21-106">For detailed information, see:</span></span>

- [<span data-ttu-id="e9f21-107">การกำหนดค่าการตั้งค่าการอัปเดตสำหรับ Office</span><span class="sxs-lookup"><span data-stu-id="e9f21-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="e9f21-108">ไม่ได้เปิดใช้งานการอัปเดตอัตโนมัติสำหรับ Office</span><span class="sxs-lookup"><span data-stu-id="e9f21-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="e9f21-109">กำหนดวิธีที่ Office ได้รับการอัปเดตหลังจากติดตั้งแล้ว</span><span class="sxs-lookup"><span data-stu-id="e9f21-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="e9f21-110">เมื่อต้องการตรวจทานการตั้งค่าการอัปเดตที่มีอยู่กับเครื่องไคลเอ็นต์ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e9f21-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="e9f21-111">เปิดตัวแก้ไขรีจิสทรีโดยไปที่**เริ่ม**  >  **เรียกใช้**  >  **regedit**</span><span class="sxs-lookup"><span data-stu-id="e9f21-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="e9f21-112">สลับไปยังตำแหน่งที่ตั้งต่อไปนี้และตรวจทานการตั้งค่าการอัปเดต Office:</span><span class="sxs-lookup"><span data-stu-id="e9f21-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="e9f21-113">a.</span><span class="sxs-lookup"><span data-stu-id="e9f21-113">a.</span></span> <span data-ttu-id="e9f21-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="e9f21-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="e9f21-115">b.</span><span class="sxs-lookup"><span data-stu-id="e9f21-115">b.</span></span> <span data-ttu-id="e9f21-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="e9f21-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="e9f21-117">**หมายเหตุ:**  ถ้ามีการตั้งค่าคีย์ OfficeMgmtCOM คุณอาจเห็นข้อความ "การอัปเดตจะถูกจัดการโดยผู้ดูแลระบบของ**Office**คุณ" ใน  >  **Account**  >  การ**อัปเดต**office บัญชี office</span><span class="sxs-lookup"><span data-stu-id="e9f21-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="e9f21-118">สำหรับข้อมูลเพิ่มเติมให้ดูที่ [จัดการการอัปเดตเป็นแอป microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า microsoft จุดสิ้น](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)สุด</span><span class="sxs-lookup"><span data-stu-id="e9f21-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  