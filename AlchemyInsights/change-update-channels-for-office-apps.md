---
title: เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4f8c1eb9d67671b5b5bef59f214b17e024227757
ms.sourcegitcommit: 847f2bfd660847440df0195258acb9253f313a69
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48949728"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="5bb13-102">เปลี่ยนช่องทางการอัปเดตสำหรับแอป Office</span><span class="sxs-lookup"><span data-stu-id="5bb13-102">Change update channels for Office apps</span></span>

<span data-ttu-id="5bb13-103">ถ้าคุณกำลังจัดการช่องทางการอัปเดตแอป Microsoft ๓๖๕โดยใช้พอร์ทัลการดูแลให้ใช้  **ตัวเลือกการติดตั้ง Office**  เพื่อเลือกแชนเนลการอัปเดตที่ต้องการก่อนที่จะติดตั้งแอป Office</span><span class="sxs-lookup"><span data-stu-id="5bb13-103">If you are managing Microsoft 365 Apps update channels using the Admin Portal, use  **Office Installation Options**  to select the desired update channel before installing Office Apps.</span></span> <span data-ttu-id="5bb13-104">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการตัวเลือกการติดตั้ง Office ในศูนย์การจัดการ Microsoft ๓๖๕](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)</span><span class="sxs-lookup"><span data-stu-id="5bb13-104">For more info, see [Manage Office installation options in the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span>

<span data-ttu-id="5bb13-105">**หมายเหตุ:** ช่องทางการอัปเดตที่เลือกโดยใช้  **ตัวเลือกการติดตั้ง Office**  จะนำไปใช้กับผู้ใช้ทุกคนที่ดำเนินการติดตั้งใหม่ (และในบางกรณีการติดตั้งที่มีอยู่แล้ว)</span><span class="sxs-lookup"><span data-stu-id="5bb13-105">**Note** The update channel selected using the  **Office Installation Options**  applies to all users performing new installations (and in certain cases, existing installations too).</span></span> <span data-ttu-id="5bb13-106">ถ้าคุณกำลังใช้วิธีอื่นๆบางอย่างเช่นเครื่องมือการปรับใช้ Office (ODT), Group policy (GPO) หรือตัวจัดการการกำหนดค่าของ Microsoft จุดสิ้นสุด (MECM) เพื่อจัดการวิธีที่ผู้ใช้ของคุณจะได้รับการอัปเดตของฟีเจอร์จากนั้นการตั้งค่าที่คุณเลือกในศูนย์การจัดการ Microsoft ๓๖๕จะไม่ถูกนำไปใช้</span><span class="sxs-lookup"><span data-stu-id="5bb13-106">If you're already using some other method, such as Office Deployment Tool (ODT), Group Policy (GPO) or Microsoft Endpoint Configuration Manager (MECM) to manage how your users get feature updates, then the settings you select in the Microsoft 365 admin center won't apply.</span></span>

<span data-ttu-id="5bb13-107">ถ้าคุณกำลังจัดการช่องทางการอัปเดต Microsoft ๓๖๕ Apps โดยใช้ตัวเลือกการจัดการอื่นๆที่แสดงรายการข้างต้นให้ดู[ที่วิธีการสลับช่องทางการอัปเดตสำหรับแอป Office ที่มีอยู่](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)</span><span class="sxs-lookup"><span data-stu-id="5bb13-107">If you are managing Microsoft 365 Apps update channels using other management options listed above, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span>

<span data-ttu-id="5bb13-108">สำหรับข้อมูลโดยละเอียดให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="5bb13-108">For detailed information, see:</span></span>  
[<span data-ttu-id="5bb13-109">วิธีการจัดการแชนแนล Office ๓๖๕ ProPlus สำหรับผู้เชี่ยวชาญด้าน IT</span><span class="sxs-lookup"><span data-stu-id="5bb13-109">How to manage Office 365 ProPlus Channels for IT Pros</span></span>](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813)  
[<span data-ttu-id="5bb13-110">จัดการการอัปเดตเป็นแอป Microsoft ๓๖๕ด้วยตัวจัดการการกำหนดค่า Microsoft จุดสิ้นสุด</span><span class="sxs-lookup"><span data-stu-id="5bb13-110">Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager</span></span>](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)