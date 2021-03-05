---
title: ปิดใช้งานการสแกนเครือข่าย
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483003"
---
# <a name="disable-network-scan"></a>ปิดใช้งานการสแกนเครือข่าย

การสแกนการแชร์เครือข่ายอาจส่งผลต่อประสิทธิภาพการคํานวณ  เพื่อให้แน่ใจว่าไคลเอ็นต์จะไม่สแกนการแชร์เครือข่าย/ไฟล์ตามค่าเริ่มต้น ให้กําหนดค่าการตั้งค่าต่อไปนี้ในแอปพลิเคชัน Windows Defender **เป็น True:**

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles