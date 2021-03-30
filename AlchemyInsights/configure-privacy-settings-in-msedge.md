---
title: กําหนดค่าการตั้งค่าความเป็นส่วนตัวใน Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405730"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="399a7-102">กําหนดค่าการตั้งค่าความเป็นส่วนตัวใน Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="399a7-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="399a7-103">ตามค่าเริ่มต้น ถ้า Microsoft Edge ถูกปรับใช้บนแพลตฟอร์มที่ไม่ใช่ Windows ข้อมูลการวินิจฉัยและข้อมูลไซต์จะไม่ส่งไปยังไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="399a7-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="399a7-104">อย่างไรก็ตาม หากมีการปรับใช้ Microsoft Edge บน Windows 10 ข้อมูลการวินิจฉัยและข้อมูลไซต์จะถูกส่งตามการตั้งค่าข้อมูล [การวินิจฉัย Windows](https://go.microsoft.com/fwlink/?linkid=2132472)ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="399a7-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="399a7-105">เมื่อต้องการกําหนดวิธีที่ Microsoft Edge จัดการการเก็บรวบรวมข้อมูลให้องค์กรของคุณ ให้ใช้นโยบายกลุ่มต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="399a7-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="399a7-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) จะเปิดการรายงานข้อมูลที่เกี่ยวข้องกับการใช้งานและการหยุดล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="399a7-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="399a7-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) ส่งข้อมูลไซต์ที่ใช้เพื่อปรับปรุงบริการของไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="399a7-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="399a7-108">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [การกําหนดค่าการตั้งค่า](https://go.microsoft.com/fwlink/?linkid=2132577)นโยบาย</span><span class="sxs-lookup"><span data-stu-id="399a7-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
