---
title: การกระทำของ Windows Defender ใน Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 732b7450121f85416bb0f1868b3722899bee8194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699106"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="54cc6-102">การกระทำของ Windows Defender ใน Intune</span><span class="sxs-lookup"><span data-stu-id="54cc6-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="54cc6-103">คุณสามารถใช้ Intune เพื่อเรียกใช้การอัปเดตที่มีการตรวจสอบความต้องการและการอัปเดตของลายเซ็นของไวรัสสำหรับ Windows Defender บนอุปกรณ์แต่ละเครื่อง</span><span class="sxs-lookup"><span data-stu-id="54cc6-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="54cc6-104">หลังจากการดำเนินการระยะไกลเสร็จสมบูรณ์แล้วทริกเกอร์กิจกรรมจะแสดงในไฟล์บันทึกเหตุการณ์ของ Windows Defender</span><span class="sxs-lookup"><span data-stu-id="54cc6-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="54cc6-105">นโยบายการป้องกันจุดสิ้นสุดของ windows อนุญาตให้มีการตั้งค่าเพิ่มเติมสำหรับฟีเจอร์ของ Windows Defender เพื่อสร้างใน Intune และนำไปใช้กับชุดของอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="54cc6-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="54cc6-106">สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการดำเนินการเรียกใช้ Windows Defender ให้ดูที่ [กำหนดค่าและเรียกใช้การสแกนป้องกันไวรัสของ Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus)ตามความต้องการ</span><span class="sxs-lookup"><span data-stu-id="54cc6-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>