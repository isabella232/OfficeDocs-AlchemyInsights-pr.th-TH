---
title: แก้ไขปัญหาเกี่ยวกับอุปกรณ์ Windows 10 แบบออนบอร์ดจากระยะไกลไปยัง Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750045"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="762bb-102">แก้ไขปัญหาเกี่ยวกับอุปกรณ์ Windows 10 แบบออนบอร์ดจากระยะไกลไปยัง Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="762bb-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="762bb-103">ถ้าคุณสามารถเข้าถึงคอมพิวเตอร์ระยะไกล ได้ ให้ปฏิบัติตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="762bb-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="762bb-104">ดาวน์โหลด [เครื่องมือวินิจฉัยการเชื่อมต่อ](https://go.microsoft.com/fwlink/?linkid=2143466) ไคลเอ็นต์</span><span class="sxs-lookup"><span data-stu-id="762bb-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="762bb-105">แยกและเรียกใช้ MDATPAnalyzer.cmd</span><span class="sxs-lookup"><span data-stu-id="762bb-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="762bb-106">ค้นหาบันทึกการวินิจฉัยในโฟลเดอร์ MDATPClientAnalyzerResult ซึ่งเป็นโฟลเดอร์เดียวกันกับที่เครื่องมือวิเคราะห์ถูกดาวน์โหลด</span><span class="sxs-lookup"><span data-stu-id="762bb-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="762bb-107">เมื่อต้องการค้นหาปัญหาเกี่ยวกับการเชื่อมต่อหรือการตั้งค่าพร็อกซีอินเทอร์เน็ต ให้รีวิวไฟล์MDATPClientAnalyzer.txt</span><span class="sxs-lookup"><span data-stu-id="762bb-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="762bb-108">เมื่อต้องการเรียนรู้เพิ่มเติม[ดูปัญหาเกี่ยวกับเครื่องออนบอร์ด](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="762bb-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
