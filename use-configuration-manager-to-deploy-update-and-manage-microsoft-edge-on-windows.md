---
title: ใช้ตัวจัดการการกำหนดค่าเพื่อปรับใช้อัปเดตและจัดการ Microsoft Edge บน Windows
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004030"
- "7100"
ms.openlocfilehash: 8987a37a1e756001c45e9407337543d70560e314
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678972"
---
# <a name="use-configuration-manager-to-deploy-update-and-manage-microsoft-edge-on-windows"></a><span data-ttu-id="18578-102">ใช้ตัวจัดการการกำหนดค่าเพื่อปรับใช้อัปเดตและจัดการ Microsoft Edge บน Windows</span><span class="sxs-lookup"><span data-stu-id="18578-102">Use Configuration Manager to deploy, update, and manage Microsoft Edge on Windows</span></span>

<span data-ttu-id="18578-103">ในฐานะที่เป็นตัวจัดการการตั้งค่าคอนฟิกเวอร์ชัน๑๙๑๐คุณสามารถปรับใช้ Microsoft Edge (เวอร์ชัน๗๗และเวอร์ชันที่ใหม่กว่า) ผ่านสคริปต์ PowerShell ได้</span><span class="sxs-lookup"><span data-stu-id="18578-103">As of Configuration Manager version 1910, you can deploy Microsoft Edge (versions 77 and later) through a PowerShell script.</span></span> <span data-ttu-id="18578-104">สคริปต์จะปิดการอัปเดตอัตโนมัติและการดำเนินการนี้จะช่วยให้คุณสามารถจัดการการอัปเดตได้ผ่านทางตัวจัดการการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="18578-104">The script turns off automatic updates, and this lets you manage the updates through Configuration Manager.</span></span> <span data-ttu-id="18578-105">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับสิ่งนี้และประโยชน์อื่นๆของการใช้ตัวจัดการการกำหนดค่าให้ดูที่[การจัดการ Microsoft Edge](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?)</span><span class="sxs-lookup"><span data-stu-id="18578-105">To learn more about this and other benefits of using Configuration Manager, see [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge?).</span></span>