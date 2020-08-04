---
title: ใช้การบันทึกการใช้งานสําหรับการจัดการสิทธิ์ Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556024"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="9373e-102">ใช้การบันทึกการใช้งานสําหรับการจัดการสิทธิ์ Azure</span><span class="sxs-lookup"><span data-stu-id="9373e-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="9373e-103">โดยค่าเริ่มต้น การบันทึกการใช้งานการป้องกันถูกเปิดใช้งานสําหรับลูกค้าทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="9373e-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="9373e-104">บันทึกถูกเขียนเป็นชุดของ blobs ในที่เก็บข้อมูล Azure สําหรับผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="9373e-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="9373e-105">หลังจากการดําเนินการป้องกันอาจใช้เวลาถึง 15 นาทีเพื่อให้บันทึกส่วนใหญ่ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="9373e-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="9373e-106">คุณสามารถใช้บันทึกการใช้งานการป้องกันเพื่อ:</span><span class="sxs-lookup"><span data-stu-id="9373e-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="9373e-107">วิเคราะห์ข้อมูลเชิงลึกทางธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="9373e-107">Analyze business insights</span></span>

- <span data-ttu-id="9373e-108">ตรวจสอบการละเมิด</span><span class="sxs-lookup"><span data-stu-id="9373e-108">Monitor for abuse</span></span>

- <span data-ttu-id="9373e-109">ดําเนินการวิเคราะห์ทางนิติเวช</span><span class="sxs-lookup"><span data-stu-id="9373e-109">Perform forensic analysis</span></span>

<span data-ttu-id="9373e-110">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การบันทึกและการวิเคราะห์การใช้งานการป้องกันจากการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)</span><span class="sxs-lookup"><span data-stu-id="9373e-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="9373e-111">สําหรับข้อมูลเกี่ยวกับการบันทึกการใช้งานไคลเอ็นต์ ให้ดูที่[คู่มือผู้ดูแลระบบ: แฟ้มไคลเอ็นต์การป้องกันข้อมูล Azure และการบันทึกการใช้งานไคลเอ็นต์](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)</span><span class="sxs-lookup"><span data-stu-id="9373e-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="9373e-112">สําหรับข้อมูลเพิ่มเติม โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="9373e-112">For additional information, see:</span></span>

- <span data-ttu-id="9373e-113">[ข้อกําหนดในการปกป้องข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span><span class="sxs-lookup"><span data-stu-id="9373e-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="9373e-114">[บทช่วยสอน: กําหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)</span><span class="sxs-lookup"><span data-stu-id="9373e-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>