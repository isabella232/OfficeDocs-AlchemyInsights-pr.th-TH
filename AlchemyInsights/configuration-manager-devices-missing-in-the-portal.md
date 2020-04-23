---
title: อุปกรณ์ตัวจัดการการตั้งค่าคอนฟิกที่ขาดหายไปในพอร์ทัล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790236"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="84fee-102">อุปกรณ์ตัวจัดการการตั้งค่าคอนฟิกที่ขาดหายไปในพอร์ทัล</span><span class="sxs-lookup"><span data-stu-id="84fee-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="84fee-103">สําหรับการซิงค์อุปกรณ์ในการทํางาน[required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)</span><span class="sxs-lookup"><span data-stu-id="84fee-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="84fee-104">เมื่อต้องการแก้ไขปัญหาการซิงค์อุปกรณ์ โปรดตรวจทาน**CMGatewaySyncUploadWorker.log**ที่อยู่บนจุดเชื่อมต่อบริการ</span><span class="sxs-lookup"><span data-stu-id="84fee-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="84fee-105">เรียนรู้เพิ่มเติมเกี่ยวกับ[ผู้เช่าที่แนบในตัวจัดการปลายทางของ Microsoft](https://docs.microsoft.com/configmgr/tenant-attach/)</span><span class="sxs-lookup"><span data-stu-id="84fee-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
