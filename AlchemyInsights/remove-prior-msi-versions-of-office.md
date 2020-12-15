---
title: เอา Office เวอร์ชันก่อนหน้านี้ออกจาก MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680778"
---
# <a name="remove-prior-msi-versions-of-office"></a>เอา Office เวอร์ชันก่อนหน้านี้ออกจาก MSI

ฉันขอแนะนำให้เอา Office Installer (MSI) เวอร์ชันก่อนหน้าก่อนที่จะติดตั้ง Office ๓๖๕ ProPlus ต่อไปนี้เป็นวิธีการทำสิ่งต่อไปนี้

1. ถ้าคุณใช้ MSI ในการติดตั้ง Office คุณสามารถใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อถอนการติดตั้ง Office ได้ คุณสามารถใช้องค์ประกอบ RemoveMSI ในไฟล์ **configuration.xml** ของคุณได้
1. ทำตามคำแนะนำในบทความนี้: [ศูนย์การรักษาความปลอดภัย & Office ๓๖๕](https://go.microsoft.com/fwlink/p/?linkid=2077143)