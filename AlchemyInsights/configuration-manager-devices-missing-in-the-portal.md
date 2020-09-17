---
title: อุปกรณ์ตัวจัดการการกำหนดค่าหายไปในพอร์ทัล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812170"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>อุปกรณ์ตัวจัดการการกำหนดค่าหายไปในพอร์ทัล

สำหรับการซิงค์อุปกรณ์กับการทำงานจุดสิ้นสุดของ [อินเทอร์เน็ตที่จำเป็น](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) ต้องสามารถเข้าถึงได้จากเซิร์ฟเวอร์ภายในองค์กรที่โฮสต์บทบาทจุดเชื่อมต่อบริการ เมื่อต้องการแก้ไขปัญหาการซิงค์อุปกรณ์โปรดตรวจทาน **CMGatewaySyncUploadWorker** ที่อยู่บนจุดเชื่อมต่อบริการ

เรียนรู้เพิ่มเติมเกี่ยวกับการ [แนบผู้เช่าในตัวจัดการจุดสิ้น](https://docs.microsoft.com/configmgr/tenant-attach/)สุดของ Microsoft
