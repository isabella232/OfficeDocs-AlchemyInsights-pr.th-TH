---
title: ควบคุมการปรับปรุงอัตโนมัติสําหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439927"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="e472e-102">ควบคุมการปรับปรุงอัตโนมัติสําหรับแอป Office</span><span class="sxs-lookup"><span data-stu-id="e472e-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="e472e-103">โดยค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="e472e-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="e472e-104">อย่างไรก็ตาม ผู้ดูแลระบบสามารถควบคุมวิธีการใช้การปรับปรุง โดยใช้การตั้งค่าการปรับปรุง Office</span><span class="sxs-lookup"><span data-stu-id="e472e-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="e472e-105">การตั้งค่าการปรับปรุงช่วยให้ผู้ดูแลระบบสามารถเปิดใช้งานหรือปิดใช้งานการปรับปรุงอัตโนมัติ**Update Now**</span><span class="sxs-lookup"><span data-stu-id="e472e-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="e472e-106">สําหรับข้อมูลโดยละเอียด โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="e472e-106">For detailed information, see:</span></span>

- [<span data-ttu-id="e472e-107">กําหนดค่าการตั้งค่าการปรับปรุงสําหรับ Office</span><span class="sxs-lookup"><span data-stu-id="e472e-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="e472e-108">การปรับปรุงอัตโนมัติสําหรับ Office ไม่ได้เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e472e-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="e472e-109">กําหนดวิธีการปรับปรุง Office หลังจากที่มีการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="e472e-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="e472e-110">เมื่อต้องการตรวจสอบการปรับปรุงที่มีอยู่การตั้งค่าที่ใช้กับเครื่องไคลเอ็นต์ ให้ทําตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="e472e-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="e472e-111">เปิดตัวแก้ไขรีจิสทรี โดยไปที่**เริ่ม**  >  **เรียกใช้**  >  **regedit**</span><span class="sxs-lookup"><span data-stu-id="e472e-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="e472e-112">สลับไปยังตําแหน่งที่ตั้งต่อไปนี้ และตรวจทานการตั้งค่าการปรับปรุง Office:</span><span class="sxs-lookup"><span data-stu-id="e472e-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="e472e-113">a.</span><span class="sxs-lookup"><span data-stu-id="e472e-113">a.</span></span> <span data-ttu-id="e472e-114">HKEY_LOCAL_MACHINE\ซอฟต์แวร์\ไมโครซอฟท์\สํานักงาน</span><span class="sxs-lookup"><span data-stu-id="e472e-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="e472e-115">b.</span><span class="sxs-lookup"><span data-stu-id="e472e-115">b.</span></span> <span data-ttu-id="e472e-116">คลิกเพื่อเรียกใช้\การกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="e472e-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="e472e-117">**หมายเหตุ**  ถ้าคีย์ OfficeMgmtCOM ถูกตั้งค่า ไว้ คุณอาจเห็นข้อความ "โปรแกรมปรับปรุงได้รับการจัดการโดยผู้ดูแลระบบของคุณ" ใน**Office**  >  **Office**  >  **Update**</span><span class="sxs-lookup"><span data-stu-id="e472e-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="e472e-118">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการการปรับปรุงแอป Microsoft 365 ด้วยตัวจัดการการตั้งค่าคอนฟิกปลายทางของ Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)</span><span class="sxs-lookup"><span data-stu-id="e472e-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  