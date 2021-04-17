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
# <a name="configuration-manager-devices-missing-in-the-portal"></a>อุปกรณ์ตัวจัดการการกําหนดค่าหายไปในพอร์ทัล

เพื่อให้การซิงค์อุปกรณ์สามารถได้ผล [จุดสิ้นสุดอินเทอร์เน็ต](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) ที่ต้องมีต้องสามารถเข้าถึงได้จากเซิร์ฟเวอร์ภายในองค์กรที่โฮสต์บทบาท จุดเชื่อมต่อบริการ เมื่อต้องการแก้ไขปัญหาการซิงค์อุปกรณ์ โปรดตรวจสอบ **CMGatewaySyncUploadWorker.log** ที่อยู่บนจุดเชื่อมต่อบริการ

เรียนรู้เพิ่มเติมเกี่ยวกับ การ [แนบผู้เช่าใน ตัวจัดการจุดสิ้นสุด](https://docs.microsoft.com/configmgr/tenant-attach/)ของ Microsoft
