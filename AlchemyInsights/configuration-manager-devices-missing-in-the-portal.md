---
title: อุปกรณ์ตัวจัดการการกําหนดค่าหายไปในพอร์ทัล
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817263"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="e396b-102">อุปกรณ์ตัวจัดการการกําหนดค่าหายไปในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="e396b-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="e396b-103">เพื่อให้การซิงค์อุปกรณ์สามารถได้ผล [จุดสิ้นสุดอินเทอร์เน็ต](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) ที่ต้องมีต้องสามารถเข้าถึงได้จากเซิร์ฟเวอร์ภายในองค์กรที่โฮสต์บทบาท จุดเชื่อมต่อบริการ</span><span class="sxs-lookup"><span data-stu-id="e396b-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="e396b-104">เมื่อต้องการแก้ไขปัญหาการซิงค์อุปกรณ์ โปรดตรวจสอบ **CMGatewaySyncUploadWorker.log** ที่อยู่บนจุดเชื่อมต่อบริการ</span><span class="sxs-lookup"><span data-stu-id="e396b-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="e396b-105">เรียนรู้เพิ่มเติมเกี่ยวกับ การ [แนบผู้เช่าใน ตัวจัดการจุดสิ้นสุด](https://docs.microsoft.com/configmgr/tenant-attach/)ของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="e396b-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
