---
title: Microsoft Edgeกําหนดค่าการตั้งค่าความเป็นส่วนตัว
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114191"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edgeกําหนดค่าการตั้งค่าความเป็นส่วนตัว

ตามค่าเริ่มต้น ถ้ามีการปรับใช้Microsoft Edgeบนแพลตฟอร์มที่ไม่ใช่แพลตฟอร์ม Windows ข้อมูลการวินิจฉัยและข้อมูลไซต์จะไม่ถูกส่งไปยัง Microsoft อย่างไรก็ตาม หากมีการปรับใช้Microsoft Edgeใน Windows 10 ข้อมูลการวินิจฉัยและข้อมูลไซต์จะถูกส่งตามการตั้งค่าข้อมูลWindows[การวินิจฉัย](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)ของผู้ใช้

เมื่อต้องการกําหนดMicrosoft Edgeจัดการการเก็บรวบรวมข้อมูลให้กับองค์กรของคุณ ให้ใช้นโยบายกลุ่มต่อไปนี้
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): นโยบายนี้จะเปิดใช้งานการรายงานการใช้และข้อมูลที่เกี่ยวข้องกับการหยุดการหยุด
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): นโยบายนี้จะส่งข้อมูลไซต์ที่ใช้เพื่อปรับปรุงการบริการของ Microsoftของคุณ

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [กําหนดค่าการตั้งค่า](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)นโยบาย