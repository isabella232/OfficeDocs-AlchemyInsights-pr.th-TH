---
title: การดําเนินการของ Windows Defender ในอินตูน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440440"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="4155b-102">การดําเนินการของ Windows Defender ในอินตูน</span><span class="sxs-lookup"><span data-stu-id="4155b-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="4155b-103">Intuner สามารถใช้เพื่อทริกเกอร์การสแกนตามความต้องการและการปรับปรุงลายเซ็นไวรัสสําหรับ Windows Defender บนอุปกรณ์แต่ละ</span><span class="sxs-lookup"><span data-stu-id="4155b-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="4155b-104">หลังจากการดําเนินการระยะไกลจะทริกเกอร์สําเร็จกิจกรรมจะสะท้อนในแฟ้มบันทึกเหตุการณ์ของ Windows Defender</span><span class="sxs-lookup"><span data-stu-id="4155b-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="4155b-105">นโยบายการป้องกันปลายทางของ Windows อนุญาตให้มีการตั้งค่าเพิ่มเติมสําหรับคุณลักษณะของ Windows Defender ที่ถูกสร้างใน Intuner และนําไปใช้กับชุดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4155b-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="4155b-106">สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเรียกใช้การกระทําของ Windows Defender โปรดดู[การกําหนดค่าและเรียกใช้การสแกนโปรแกรมป้องกันไวรัสของ Microsoft Defender ตามความต้องการ](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="4155b-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>