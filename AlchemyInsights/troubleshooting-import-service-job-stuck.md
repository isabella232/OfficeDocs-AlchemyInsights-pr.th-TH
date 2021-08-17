---
title: การแก้ไขปัญหาการนําเข้างานบริการค้าง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105119"
---
# <a name="troubleshooting-import-service-job-stuck"></a>การแก้ไขปัญหาการนําเข้างานบริการค้าง

ถ้าคุณพบปัญหาเกี่ยวกับการนําเข้างานบริการค้างหรือล้มเหลว ให้ตรวจสอบและลองใช้วิธีต่อไปนี้

- ตรวจสอบขนาดของไฟล์ PST ขนาดสูงสุดที่แนะนําของไฟล์ PST เพื่อนําเข้าคือ 20 GB

- ถ้าคุณสงสัยรายการที่ข้ามเนื่องจากความเสียหาย ให้เรียกใช้Scanpst.exeวินิจฉัยและแก้ไขข้อผิดพลาดในไฟล์ PST

- ถ้าคุณเห็นข้อผิดพลาด "MapiExceptionShutoffQuotaExceeded" ระหว่างการนําเข้า ให้ตรวจสอบให้แน่ใจว่ากล่องจดหมายเป้าหมายมีความจุเพียงพอที่จะนําเข้าไฟล์ PST ที่ต้องการ

For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

For information about how to fix issues when importing PSTs into Outlook, [see Fix problems importing an Outlook .pst (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).